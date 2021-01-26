---
title: Problemas de autenticação
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976837"
---
# <a name="authentication-issues"></a>Problemas de autenticação

**Procurando informações sobre os códigos de erro AADSTS retornados do serviço de token de segurança (STS) do Azure Active Directory (Azure AD)?** Confira [códigos de erro de autorização e autenticação do Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) para encontrar descrições de erros, correções e algumas soluções alternativas sugeridas para AADSTS.

Os erros de autorização podem ocorrer como resultado de vários problemas diferentes, a maioria dos quais gera um erro 401 ou 403. Por exemplo, todos os problemas a seguir podem levar a erros de autorização:

- [Fluxos de aquisição de token de acesso](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) incorretos 
- [Escopos de permissão](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) mal configurados 
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Para resolver erros comuns de autorização, tente as etapas fornecidas a seguir que mais se aproximam do erro que está ocorrendo. Mais de uma etapa pode se aplicar a um erro que você está recebendo.

**Erro 401 Não autorizado: seu token é válido?**

Verifique se o aplicativo está apresentando um token de acesso válido ao Microsoft Graph como parte da solicitação. Esse erro geralmente significa que o token de acesso pode estar ausente no cabeçalho da solicitação de autenticação HTTP, ou que o token é inválido ou expirou. É altamente recomendável o uso da MSAL (Biblioteca de Autenticação da Microsoft) para aquisição de tokens de acesso. Além disso, esse erro pode ocorrer ao tentar usar um token de acesso delegado concedido a uma conta pessoal da Microsoft, para acessar uma API que só dê suporte a contas corporativas ou de estudante (contas organizacionais).

**Erro 403 Proibido: você escolheu o conjunto certo de permissões?**

Verifique se você solicitou o conjunto correto de permissões com base nas APIs do Microsoft Graph que seu aplicativo chama. As permissões menos privilegiadas recomendadas são fornecidas em todos os tópicos do método de referência da API do Microsoft Graph. Além disso, essas permissões devem ser concedidas ao aplicativo por um usuário ou administrador. A concessão de permissões normalmente acontece por meio de uma página de consentimento ou pelo uso da folha de registro do aplicativo do Portal Azure. Na folha **Configurações** do aplicativo, clique em **Permissões necessárias** e, em seguida, clique em **Conceder permissões**. Para mais informações, confira:

- [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Noções básicas sobre permissões e consentimento do Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Erro 403 Proibido: seu aplicativo adquiriu um token para corresponder às permissões escolhidas?**

Verifique se os tipos de permissões solicitadas ou concedidas correspondem ao tipo de token de acesso das aquisições do aplicativo. Você pode estar solicitando e concedendo permissões de aplicativos, mas usando tokens de fluxo de código interativo delegado, em vez de tokens de fluxo de credencial de cliente, ou solicitando e concedendo permissões delegadas, mas usando tokens de fluxo de credencial de cliente em vez de tokens de fluxo de código delegado.

Para obter mais informações relacionadas à aquisição de tokens, veja:

- [Obtenha acesso em nome de usuários e permissões delegadas](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obter acesso sem um usuário (serviço daemon) e permissões de aplicativo](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - fluxo de credenciais do cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Erro 403 Proibido: redefinindo a senha**

No momento, não há permissões de serviço a serviço de permissão de aplicativo daemon que permitam a redefinição de senhas dos usuários. Essas APIs têm suporte somente usando os fluxos de código delegados interativos com um administrador conectado. Para obter mais informações, veja [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 Proibido: o usuário tem acesso e está licenciado?**

Para fluxos de código delegado, o Microsoft Graph avalia se a solicitação é permitida com base nas permissões concedidas ao aplicativo e nas permissões que o usuário conectado tem. Geralmente, esse erro indica que o usuário não tem privilégio suficiente para executar a solicitação **ou** não está licenciado para os dados que estão sendo acessados. Somente os usuários com as permissões ou licenças necessárias podem fazer a solicitação com êxito.

**403 Proibido: você selecionou a API de recurso correta?**

Serviços de API, como o Microsoft Graph, verificam se a declaração de *aud* (audiência) no token de acesso recebido corresponde ao valor esperado para si e, caso contrário, ocorrerá um erro 403 Proibido. Um equívoco comum que resulta nesse erro é tentar usar um token adquirido para APIs do Azure AD Graph, APIs do Outlook, ou APIs do SharePoint/OneDrive para chamar o Microsoft Graph (ou vice-versa). Verifique se o recurso (ou escopo) para o qual o seu aplicativo está adquirindo um token corresponde à API que o aplicativo está chamando.

**400 Solicitação incorreta ou 403 Proibido: o usuário está em conformidade com as políticas de acesso condicional (CA) da organização?**

Com base nas políticas de CA (acesso condicional) de uma organização, um usuário que acesse os recursos do Microsoft Graph por meio do aplicativo pode ser desafiado a obter informações adicionais que não estejam presentes no token de acesso que o aplicativo adquiriu originalmente. Nesse caso, o aplicativo recebe um **400 com um erro de *interaction_required*** durante a aquisição do token de acesso ou um **403 com erro de *insufficient_claims*** ao chamar o Microsoft Graph. Em ambos os casos, a resposta ao erro contém informações adicionais que podem ser apresentadas ao ponto de extremidade autorizado para desafiar o usuário a obter informações adicionais (como autenticação multifator ou registro do dispositivo).

Para obter mais informações relacionadas ao acesso condicional, veja:

- [Lidar com desafios de acesso condicional usando a MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Orientações do desenvolvedor para acesso condicional do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Fim do suporte à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph)_* _

- A partir de 30 de junho de 2020, não adicionaremos mais nenhum novo recurso à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph). Continuaremos dando suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.
- A partir de 30 de junho de 2022, encerraremos o suporte à ADAL e à AAD Graph, e não forneceremos mais suporte técnico ou atualizações de segurança.
    - Os aplicativos que usam a ADAL nas versões existentes do sistema operacional continuarão a funcionar após esse período, mas não receberão nenhum suporte técnico ou atualizações de segurança.
    - Os aplicativos que usarem o AAD Graph após esse período, talvez não recebam mais respostas do ponto de extremidade do AAD Graph.

_ *Migração da ADAL**

Recomendamos a atualização para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem os últimos recursos e as atualizações de segurança. Essa recomendação está no contexto da migração de aplicativos da Microsoft para a MSAL até o prazo final de suporte. O objetivo da migração de aplicativos da Microsoft para a MSAL é garantir que os aplicativos se beneficiem das melhorias contínuas nos recursos e na segurança da MSAL.

- [Leia as perguntas frequentes sobre a ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Saiba mais sobre como migrar aplicativos por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Se precisar de ajuda para entender qual de seus aplicativos usa a ADAL, recomendamos que você reveja todos o códigos-fonte dos aplicativos; se aplicável, procure por provedores independentes de software (ISVs) ou por provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.

**Migração do AAD Graph**

Para os aplicativos que usam o AAD Graph, siga nossa orientação para [migrar os aplicativos do Azure AD Graph para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Nossa lista de verificação de migração fornece um ponto de partida](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph. Recomendamos que você reveja todos o códigos- fonte de seu aplicativos e, se aplicável, contate os ISVs ou os provedores de aplicativos. O suporte da Microsoft também pode fornecer as informações de todos os usos do AAD Graph no seu locatário.

 











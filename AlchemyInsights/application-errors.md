---
title: Erros de aplicativo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976875"
---
# <a name="application-errors"></a>Erros de aplicativo

Procurando informações sobre os códigos de erro do **AADSTS** que são retornados do STS (serviço de token de segurança) do Azure Active Directory (Azure AD)? Leia os códigos de erro de autenticação e autorização do [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) para encontrar descrições, correções e algumas soluções alternativas sugeridas.

Erros de autorização podem ser resultado de vários problemas diferentes, a maioria dos quais gera um erro 401 ou 403. Por exemplo, todos os itens a seguir podem levar a erros de autorização:

- [Fluxos de aquisição de token de acesso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorretos 
- [Escopos de permissão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurados 
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Para resolver erros comuns de autorização, tente as etapas fornecidas abaixo que mais se aproximam do erro que você está recebendo. Mais de um pode ser aplicado.

**Erro 401 Não autorizado: seu token é válido?**

Certifique-se de que seu aplicativo está apresentando um token de acesso válido ao Microsoft Graph como parte da solicitação. Esse erro geralmente significa que o token de acesso pode estar ausente no cabeçalho da solicitação de autenticação HTTP, ou que o token é inválido ou expirou. É altamente recomendável que você use a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) para aquisição de tokens de acesso. Além disso, esse erro poderá ocorrer se você tentar usar um token de acesso delegado concedido a uma conta pessoal da Microsoft para acessar uma API que só dá suporte a contas de trabalho ou de estudante (contas organizacionais).

**Erro 403 Proibido: você escolheu o conjunto certo de permissões?**

Verifique se você solicitou o conjunto correto de permissões com base nas APIs do Microsoft Graph que seu aplicativo chama. Permissões menos privilegiadas recomendadas são fornecidas em todos os tópicos do método de referência da API do Microsoft Graph. Além disso, essas permissões devem ser concedidas ao aplicativo por um usuário ou administrador. A concessão de permissões normalmente acontece por meio de uma página de consentimento, ou pela concessão de permissões usando a folha de registro do aplicativo Portal do Azure. Na folha **Configurações** do aplicativo, clique em **Permissões necessárias** e, em seguida, clique em **Conceder permissões**.

- [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Noções básicas sobre permissões e consentimento do Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Erro 403 Proibido: seu aplicativo adquiriu um token para corresponder às permissões escolhidas?**

Certifique-se de que o tipo de permissão solicitado ou concedido corresponda ao tipo de token de acesso que seu aplicativo adquire. Você pode estar solicitando e concedendo permissões do aplicativo, mas usando tokens de fluxo de código interativo delegados, em vez de tokens de fluxo de credencial de cliente, ou solicitando e concedendo permissões delegadas, mas usando tokens de fluxo de credenciais de cliente em vez de tokens de fluxo de código delegados.

- [Obtenha acesso em nome de usuários e permissões delegadas](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obter acesso sem um usuário (serviço daemon) e permissões de aplicativo](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - fluxo de credenciais do cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Erro 403 Proibido: redefinindo a senha**

No momento, não há permissões de serviço a serviço de permissão de aplicativo daemon que permitam a redefinição de senhas dos usuários. Essas APIs têm suporte somente usando os fluxos de código delegados interativos com um administrador conectado.

- [Permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Proibido: o usuário tem acesso e está licenciado?**

Para fluxos de código delegados, o Microsoft Graph avalia se a solicitação é permitida com base nas permissões concedidas ao aplicativo e nas permissões que o usuário entrar tem. Geralmente, esse erro indica que o usuário não tem privilégio suficiente para executar a solicitação ou não está licenciado para os dados que estão sendo acessados. Somente os usuários com as permissões ou licenças necessárias podem fazer a solicitação com êxito.

**403 Proibido: você selecionou a API de recurso correta?**

Serviços de API como o Microsoft Graph verificam se a declaração de aud (audiência) no token de acesso recebido corresponde ao valor que ele espera para si mesmo e, caso não tenha, isso resulta em um erro 403 Proibido. Um erro comum que resulta nesse erro é tentar usar um token adquirido para APIs do Azure AD Graph, APIs do Outlook ou APIs do SharePoint/OneDrive para chamar o Microsoft Graph (ou vice-versa). Verifique se o recurso (ou escopo) para o qual o seu aplicativo está adquirindo um token corresponde à API que o aplicativo está chamando.

**400 Solicitação incorreta ou 403 Proibido: o usuário está em conformidade com as políticas de acesso condicional (CA) da organização?**

Com base nas políticas de AC de uma organização, um usuário que acessa os recursos do Microsoft Graph por meio de seu aplicativo pode ser desafiado a obter informações adicionais que não estão presentes no token de acesso que seu aplicativo adquiriu originalmente. Nesse caso, seu aplicativo recebe um 400 com um erro *interaction_required* durante a aquisição de token de acesso, ou um 403 com o erro *insufficient_claims* ao chamar o Microsoft Graph. Em ambos os casos, a resposta ao erro contém informações adicionais que podem ser apresentadas ao ponto de extremidade de autorização para desafiar o usuário a obter informações adicionais (como autenticação multifator ou registro do dispositivo).

- [Lidar com desafios de acesso condicional usando MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Orientações do desenvolvedor para acesso condicional do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)

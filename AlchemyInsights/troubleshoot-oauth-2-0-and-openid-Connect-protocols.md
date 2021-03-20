---
title: Solucionar problemas dos protocolos OAuth 2.0 e OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897454"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Solucionar problemas dos protocolos OAuth 2.0 e OpenID Connect

Para resolver os problemas do OAuth 2.0 e do OpenID Connect, execute as seguintes etapas recomendadas:

Confira os artigos a seguir relacionados à configuração e solução de problemas dos protocolos OAuth 2.0 e OpenID Connect:

- [Plataforma de identidade para desenvolvedores da Microsoft e fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Este artigo descreve como programar diretamente no **fluxo de concessão de código (PKCE)** em seu aplicativo usando qualquer idioma.
- [Plataforma de identidade para desenvolvedores da Microsoft e fluxo de credenciais do cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Este artigo descreve como programar diretamente no **fluxo de credenciais do cliente** em seu aplicativo.
- [Plataforma de identidade para desenvolvedores da Microsoft e Credenciais de Senha de Proprietário do Recurso do OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – Este artigo descreve como programar diretamente no **fluxo do ROPC** em seu aplicativo.
    - A plataforma de identidade para desenvolvedores da Microsoft só dá suporte ao ROPC para locatários do Azure AD, e não para contas pessoais. Isso significa que você deve usar um ponto de extremidade específico do locatário **(https://login.microsoftonline.com/{TenantId_or_Name})** ou o ponto de extremidade da **organização**.
    - As contas pessoais que são convidadas a um locatário do Azure AD não podem usar o ROPC.
    - As contas que não têm senhas não podem entrar por meio do ROPC. Para esse cenário, recomendamos que você use um fluxo diferente para o seu aplicativo.
    - Se os usuários precisarem usar a [MFA (autenticação multifator)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) para entrar no aplicativo, eles serão bloqueados.
    - O ROPC não tem suporte em [cenários de federação de identidade híbrida](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (por exemplo, o Azure AD e o ADFS usados para autenticar contas locais). Se os usuários forem redirecionados de uma página inteira para um provedor de identidade no local, o Azure AD não conseguirá testar o nome de usuário e a senha no provedor de identidade. No entanto, a [autenticação de passagem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) é compatível com o ROPC.
    - Uma exceção a um cenário de federação de identidade híbrida seria o seguinte: a política Descoberta de Realm Inicial com **AllowCloudPasswordValidation** definida como **TRUE** habilitará o fluxo do ROPC para funcionar para usuários federados quando a senha local for sincronizada com a nuvem. Para saber mais, confira [Habilitar a autenticação de ROPC direta de usuários federados para aplicativos herdados](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Plataforma de identidade para desenvolvedores da Microsoft e fluxo On-Behalf-Of do OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – Este artigo descreve como programar diretamente no **fluxo On-Behalf-Of (OBO)** em seu aplicativo.
- [Plataforma de identidade para desenvolvedores da Microsoft e protocolo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Este artigo mostra como implementar o protocolo OpenID Connect independente do idioma, e descreve como enviar e receber mensagens HTTP sem usar bibliotecas de código aberto da Microsoft.

**Tokens de Acesso**

[Tokens de acesso à plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Saiba como sua API pode validar e usar as declarações dentro de um token de acesso. Toda a documentação nesse artigo, exceto quando indicado, aplica-se somente aos tokens emitidos para APIs que você registrou. Isso não se aplica aos tokens emitidos para APIs de propriedade da Microsoft; esses tokens também não podem ser usados para validar como faz a plataforma de identidade da Microsoft ao emitir tokens para uma API que você cria.

**Configuração do Aplicativo**

[Restrições e limitações do URI de Redirecionamento (URL de resposta)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Saiba como configurar seu URI de Redirecionamento (URL de resposta). Um URI de redirecionamento, ou URL de resposta, é o local onde o servidor de autorização envia o usuário uma vez que o aplicativo tenha sido autorizado com êxito, e tenha sido concedido um código de autorização ou um token de acesso. O servidor de autorização envia o código ou token para o URI de redirecionamento; por isso é importante que você registre o local correto, como parte do processo de registro do aplicativo.

**Provisionamento de Aplicativo**

[Tutorial: Desenvolver e planejar o provisionamento para um ponto de extremidade SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – Este artigo descreve como construir um ponto de extremidade SCIM e integrá-lo ao serviço de provisionamento do AAD.



---
title: Solucionar problemas de SSO (SSO) baseado em OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726904"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Solucionar problemas de SSO (SSO) baseado em OIDC

- Para saber como adicionar um aplicativo baseado em OIDC ao locatário do Azure, consulte Início rápido: Configurar o SSO (logon único) baseado em OIDC para um aplicativo no locatário do [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Para obter mais detalhes sobre aplicativos que usam o padrão OpenID Connect para implementar o login único, consulte [Understand OIDC-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Para obter informações caso você escolha escrever seu código enviando e manipulando diretamente solicitações HTTP ou usando uma biblioteca de código aberto de terceiros, em vez de usar uma de nossas bibliotecas de código aberto, consulte [protocolos OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)e OpenID Connect na plataforma de identidade da Microsoft.

**Protocolos**

1. [Plataforma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) de identidade da Microsoft e fluxo de concessão implícito - A característica de definição da concessão implícita é que tokens (tokens de ID ou tokens de acesso) são retornados diretamente do ponto de extremidade /autorizar em vez do ponto de extremidade /token. Isso é frequentemente usado como parte do fluxo de código de autorização, no que é chamado de "fluxo híbrido" - recuperar o token de ID na **solicitação /autorizar** juntamente com um código de autorização . Este artigo descreve como programar diretamente em relação ao protocolo em seu aplicativo para solicitar tokens do Azure AD.
2. [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - The OAuth 2.0 authorization code grant can be used in apps that are installed on a device to gain access to protected resources, such as web APIs. Usando a implementação da plataforma de identidade da Microsoft do OAuth 2.0, você pode adicionar entrada e acesso à API aos seus aplicativos móveis **e de área de trabalho.** Este artigo descreve como programar diretamente em relação ao protocolo em seu aplicativo usando qualquer idioma.
3. Plataforma de identidade da Microsoft e protocolo [OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Quando você usa a implementação da plataforma de identidade da Microsoft do OpenID Connect, você pode adicionar entrada e acesso à API aos seus aplicativos. Este artigo mostra como fazer isso independentemente do idioma e descreve como enviar e receber mensagens HTTP sem usar bibliotecas de código aberto **da Microsoft.**
4. Plataforma de identidade da Microsoft e o fluxo de credenciais do cliente [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Você pode usar a concessão de credenciais de cliente OAuth 2.0 especificadas no RFC 6749, às vezes chamada **de OAuth** de duas patas, para acessar recursos hospedados na Web usando a identidade de um aplicativo. Esse tipo de concessão é comumente usado para interações de servidor para servidor que devem ser executados em segundo plano, sem interação imediata com um usuário. Esses tipos de aplicativos são geralmente chamados de **daemons** ou **contas de serviço.** Este artigo descreve como programar diretamente em relação ao protocolo em seu aplicativo.

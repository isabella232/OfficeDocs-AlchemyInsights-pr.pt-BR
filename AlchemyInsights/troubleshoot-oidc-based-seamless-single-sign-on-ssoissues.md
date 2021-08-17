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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105748"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Solucionar problemas de SSO (SSO) baseado em OIDC

- Para saber como adicionar um aplicativo baseado em OIDC ao locatário do Azure, consulte Início rápido: Configurar o SSO (logon único) baseado em OIDC para um aplicativo no locatário do [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Para obter mais detalhes sobre aplicativos que usam o Conexão OpenID para implementar o login único, consulte [Understand OIDC-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Para obter informações caso você escolha escrever seu código enviando e manipulando diretamente solicitações HTTP ou usando uma biblioteca de código aberto de terceiros, em vez de usar uma de nossas bibliotecas de código aberto, consulte [protocolos OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)e OpenID Conexão no plataforma de identidade da Microsoft .

**Protocolos**

1. [plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) e fluxo de concessão implícito - A característica de definição da concessão implícita é que tokens (tokens de ID ou tokens de acesso) são retornados diretamente do ponto de extremidade /autorizar em vez do ponto de extremidade /token. Isso é frequentemente usado como parte do fluxo de código de autorização, no que é chamado de "fluxo híbrido" - recuperar o token de ID na **solicitação /autorizar** juntamente com um código de autorização . Este artigo descreve como programar diretamente em relação ao protocolo em seu aplicativo para solicitar tokens do Azure AD.
2. plataforma de identidade da Microsoft e fluxo de código de autorização do [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - A concessão de código de autorização do OAuth 2.0 pode ser usada em aplicativos instalados em um dispositivo para obter acesso a recursos protegidos, como APIs da Web. Usando a plataforma de identidade da Microsoft implementação do OAuth 2.0, você pode adicionar entrada e acesso à API aos seus aplicativos móveis **e de área de trabalho.** Este artigo descreve como programar diretamente em relação ao protocolo em seu aplicativo usando qualquer idioma.
3. [plataforma de identidade da Microsoft e protocolo Conexão OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Quando você usa a implementação do plataforma de identidade da Microsoft openid Conexão, você pode adicionar entrada e acesso à API aos seus aplicativos. Este artigo mostra como fazer isso independentemente do idioma e descreve como enviar e receber mensagens HTTP sem usar bibliotecas de código aberto **da Microsoft.**
4. plataforma de identidade da Microsoft e o fluxo de credenciais do cliente [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Você pode usar as credenciais de cliente OAuth 2.0 especificadas no RFC 6749, às vezes chamada **de OAuth** de duas patas, para acessar recursos hospedados na Web usando a identidade de um aplicativo. Esse tipo de concessão é comumente usado para interações de servidor para servidor que devem ser executados em segundo plano, sem interação imediata com um usuário. Esses tipos de aplicativos são geralmente chamados de **daemons** ou **contas de serviço.** Este artigo descreve como programar diretamente em relação ao protocolo em seu aplicativo.

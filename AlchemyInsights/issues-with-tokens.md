---
title: Problemas com os tokens
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911968"
---
# <a name="issues-with-tokens"></a>Problemas com os tokens

Para resolver problemas relacionados aos tokens, execute as seguintes etapas:

1. Você pode especificar o tempo de vida de um acesso, ID ou token de SAML emitido pela plataforma de identidade da Microsoft. É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização. Para mais informações sobre como fazer isso, consulte [Vida útil do token configurável na plataforma de identidade da Microsoft (pré-visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Os tokens de acesso permitem que os clientes chamem com segurança APIs da web protegidas e são usados por APIs da web para realizar autenticação e autorização. De acordo com a especificação OAuth, os tokens de acesso são strings opacas sem um formato definido - alguns provedores de identidade (IDPs) usam GUIDs, outros usam blobs criptografados. A plataforma de identidade da Microsoft usa uma variedade de formatos de token de acesso, dependendo da configuração da API que aceita o token. Para saber como sua API pode validar e usar as declarações dentro de um token de acesso, consulte [Tokens de acesso à plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. A Microsoft Authentication Library (MSAL) oferece suporte a vários fluxos de autenticação para uso em diferentes cenários de aplicativos. Para obter mais informações, consulte [Fluxos de autenticação](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. A concessão do código de autorização OAuth 2.0 pode ser usada em aplicativos instalados em um dispositivo para obter acesso a recursos protegidos, como APIs da web. Usando a implementação da plataforma de identidade da Microsoft do OAuth 2.0, você pode adicionar login e acesso à API aos seus aplicativos móveis e de desktop. Consulte a [plataforma de identidade para desenvolvedores da Microsoft e o fluxo do código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) para saber como programar diretamente no protocolo em seu aplicativo, usando qualquer idioma.
5. OpenID Connect (OIDC) é um protocolo de autenticação baseado em OAuth 2.0 que você pode usar para conectar um usuário a um aplicativo com segurança. Ao usar a implementação do ponto de extremidade da plataforma de identidade da Microsoft do OpenID Connect, você pode adicionar login e acesso à API aos seus aplicativos. [A plataforma de identidade da Microsoft e o protocolo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) mostram como fazer isso independentemente do idioma e descreve como enviar e receber mensagens HTTP sem usar nenhuma biblioteca de código aberto da Microsoft.
    - O ponto de extremidade UserInfo faz parte do padrão OIDC, projetado para retornar declarações sobre o usuário que foi autenticado. Para obter mais informações, confira a [plataforma de identidade para desenvolvedores da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - O exemplo [Chamando uma API da web em um aplicativo da web usando o Microsoft Azure Active Directory e OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) mostra como criar um aplicativo da web MVC que usa o Azure AD para entrar usando o protocolo OpenID Connect e, em seguida, chamar uma API da web sob o usuário conectado identidade usando tokens obtidos por meio do OAuth 2.0. Este exemplo usa o middleware OpenID Connect ASP .Net OWIN e ADAL .Net.
6. [Configure um aplicativo para expor uma API da web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) - neste início rápido, você registra uma API da web com a plataforma de identidade da Microsoft e a expõe aos aplicativos cliente adicionando um escopo de exemplo. Ao registrar sua API da web e expô-la por meio de escopos, você pode fornecer acesso baseado em permissões a seus recursos para usuários autorizados e aplicativos cliente que acessam sua API.
7. No Azure Active Directory B2C (Azure AD B2C), o fluxo de credenciais de senha do proprietário do recurso (ROPC) é um fluxo de autenticação padrão OAuth. Nesse fluxo, um aplicativo, também conhecido como parte confiável, troca credenciais válidas por tokens. As credenciais incluem um ID de usuário e senha. Os tokens retornados são um token de ID, um token de acesso e um token de atualização. Para obter mais informações, consulte [Configurar um fluxo de credenciais de senha de proprietário de recurso no Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 


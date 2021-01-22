---
title: Problemas de conexão SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49918133"
---
# <a name="sso-connection-issues"></a>Problemas de conexão SSO

1. Siga o [ Guia de Início Rápido: Configurar propriedades para um ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guia de aplicativo para configurar seu aplicativo.
2. Dependendo do aplicativo e [da opção de logor único](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) escolhido, siga as orientações apropriadas abaixo:
    - Para configurar  um aplicativo local para o single sign-on baseado em **SAML,** consulte o single [sign-on SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)para aplicativos locais com o Proxy de Aplicativo.
    - Para configurar um **aplicativo de nuvem** para o acesso único baseado **em senha,** consulte [Configurar o single sign-on de senha.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Para configurar um **aplicativo local** para o single **sign-on** por meio do Proxy de Aplicativo, consulte Cofre de senhas para o single [sign-on com o Proxy de Aplicativo.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Solução** de problemas do Proxy de Aplicativo: recomendamos que você comece a analisar o fluxo de solução de problemas, [depurar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemas do Conector de Proxy de Aplicativo para determinar se os conectores de Proxy de Aplicativo estão configurados corretamente. Se você ainda estiver tendo problemas para se conectar ao aplicativo, siga o fluxo de solução de problemas nos problemas do aplicativo Proxy de Aplicativo [de Depuração.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Você pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) usando as ferramentas de depuração do navegador:
    - Inicie o navegador e navegue até o aplicativo da web.
    - Pressione **F12** para abrir o console de depuração.
    - Tente reproduzir a transação e revise a mensagem do console. Uma violação do CORS produz um erro de console sobre a origem.
    - Alguns problemas de CORS não podem ser resolvidos, como quando seu aplicativo redireciona para o login.microsoft.com autenticar e o token de acesso expira. Em seguida, a chamada CORS falha. Uma solução alternativa para este cenário é estender a vida útil do token de acesso, para evitar que ele expire durante a sessão de um usuário. Para mais informações sobre como fazer isso, consulte [Vida útil do token configurável na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Solução de problemas do single **sign-on** baseado em SAML: recomendamos verificar problemas ao entrar em aplicativos configurados com base em SAML single [sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)para encontrar as soluções para os problemas que você provavelmente encontrará.
5. Solução de problemas de single **sign-on** baseado em senha: recomendamos verificar a solução de problemas de single sign-on baseado em senha no [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)para encontrar as soluções para os problemas que você provavelmente encontrará.
6. Para problemas de conexão ao usar uma VPN, consulte Como usar o [SSO (single sign on) via VPN e Wi-Fi conexões.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)

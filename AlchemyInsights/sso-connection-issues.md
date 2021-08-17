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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084334"
---
# <a name="sso-connection-issues"></a>Problemas de conexão SSO

1. Siga o [ Guia de Início Rápido: Configurar propriedades para um ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guia de aplicativo para configurar seu aplicativo.
2. Dependendo do aplicativo e [da opção de logom único](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) que você escolheu, siga as diretrizes apropriadas abaixo:
    - Para configurar um aplicativo **local** para o login único baseado em **SAML,** consulte [SAML single-sign-on for](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)local applications with Application Proxy .
    - Para configurar um **aplicativo de nuvem** **para o login único** baseado em senha, consulte Configure password single  [sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Para configurar um **aplicativo local** para um único login por meio do **Proxy** de Aplicativo, consulte [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Solução de** problemas de Proxy de Aplicativo : recomendamos que você comece a revisar o fluxo de solução de problemas, [depurar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemas do Conector de Proxy de Aplicativo, para determinar se os conectores de Proxy de Aplicativo estão configurados corretamente. Se você ainda estiver com problemas para se conectar ao aplicativo, siga o fluxo de solução de problemas em Problemas do aplicativo Proxy de [Depuração.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Você pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) usando ferramentas de depuração do navegador:
    - Inicie o navegador e navegue até o aplicativo da web.
    - Pressione **F12** para abrir o console de depuração.
    - Tente reproduzir a transação e revise a mensagem do console. Uma violação do CORS produz um erro de console sobre a origem.
    - Alguns problemas do CORS não podem ser resolvidos, como quando o aplicativo redireciona para login.microsoft.com autenticar e o token de acesso expira. Em seguida, a chamada CORS falha. Uma solução alternativa para este cenário é estender a vida útil do token de acesso, para evitar que ele expire durante a sessão de um usuário. Para mais informações sobre como fazer isso, consulte [Vida útil do token configurável na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Solução de problemas de login único baseado em **SAML:** recomendamos verificar Problemas de login em aplicativos configurados com base em [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)para encontrar as soluções para os problemas que você provavelmente encontrará.
5. **Solução de** problemas de login único baseado em senha: recomendamos verificar Solução de problemas de login único baseado em senha no [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)para encontrar as soluções para os problemas que você provavelmente encontrará.
6. Para problemas de conexão ao usar uma VPN, consulte [How to use single sign on (SSO) over VPN and Wi-Fi connections](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).

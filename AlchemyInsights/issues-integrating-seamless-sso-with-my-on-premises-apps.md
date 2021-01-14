---
title: Problemas com a integração do SSO Contínuo com meus aplicativos locais
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848766"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemas com a integração do SSO Contínuo com meus aplicativos locais

Para solucionar problemas com a integração do SSO Contínuo com aplicativos locais, faça o seguinte:

**Etapas recomendadas**

1. Para configurar um **aplicativo local** para o single **sign-on** por meio do Proxy de Aplicativo, consulte Cofre de senhas para o single [sign-on com o Proxy de Aplicativo.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Solução** de problemas do Proxy de Aplicativo: recomendamos que você comece a analisar o fluxo de solução de problemas, [depurar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemas do Conector de Proxy de Aplicativo para determinar se os conectores de Proxy de Aplicativo estão configurados corretamente. Se você ainda estiver tendo problemas para se conectar ao aplicativo, siga as etapas de solução de problemas em [Depurar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)problemas de aplicativo proxy de aplicativo. Você pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) usando as seguintes ferramentas de depuração do navegador:
    1. Iniciar o navegador e navegar até o aplicativo Web.
    1. Pressione **F12** para abrir o console de depuração.
    1. Tente reproduzir a transação e revise a mensagem do console. Uma violação do CORS produz um erro de console sobre a origem.
    1. Alguns problemas de CORS não podem ser resolvidos, como quando seu aplicativo redireciona para login.microsoftonline.com autenticar e o token de acesso expira. Em seguida, a chamada CORS falha. Uma solução alternativa para esse cenário é estender o tempo de vida do token de acesso, para evitar que ele expire durante a sessão de um usuário. Para obter mais informações sobre como fazer isso, consulte Tempo de vida [de token configurável na Plataforma de Identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Documentos Recomendados**

- [Como configurar o single sign-on para um aplicativo proxy de aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML single sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Entender e resolver problemas de CORS do Proxy de Aplicativo do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Solucionar problemas de configurações de delegação restrita de Kerberos para Proxy de Aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
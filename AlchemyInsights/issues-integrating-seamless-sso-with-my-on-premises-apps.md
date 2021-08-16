---
title: Problemas com a integração do SSO contínuo com meus aplicativos locais
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028280"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemas com a integração do SSO contínuo com meus aplicativos locais

Para solucionar problemas com a integração do SSO contínuo com aplicativos locais, faça o seguinte:

**Etapas recomendadas**

1. Para configurar um **aplicativo local** para um único login por meio do **Proxy** de Aplicativo, consulte [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Solução de** problemas de Proxy de Aplicativo : recomendamos que você comece a revisar o fluxo de solução de problemas, problemas do Conector de Proxy de Aplicativo de [Depuração,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)para determinar se os conectores de Proxy de Aplicativo estão configurados corretamente. Se você ainda tiver problemas para se conectar ao aplicativo, siga as etapas de solução de problemas em [ Depurar problemas do aplicativo Proxy do Aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Você pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) usando as seguintes ferramentas de depuração do navegador:
    1. Inicie o navegador e navegue até o aplicativo da web.
    1. Pressione **F12** para abrir o console de depuração.
    1. Tente reproduzir a transação e revise a mensagem do console. Uma violação do CORS produz um erro de console sobre a origem.
    1. Alguns problemas do CORS não podem ser resolvidos, como quando o aplicativo redireciona para login.microsoftonline.com autenticar e o token de acesso expira. Em seguida, a chamada CORS falha. Uma solução alternativa para este cenário é estender a vida útil do token de acesso, para evitar que ele expire durante a sessão de um usuário. Para mais informações sobre como fazer isso, consulte [Vida útil do token configurável na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Documentos Recomendados**

- [Como configurar o login único em um aplicativo Proxy de Aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Login único SAML para aplicativos locais com Proxy de Aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Compreender e resolver Azure Active Directory cors do proxy de aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Solução de problemas de configurações de delegação restrita de Kerberos para Proxy de Aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
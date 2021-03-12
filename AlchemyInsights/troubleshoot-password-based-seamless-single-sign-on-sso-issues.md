---
title: Solucionar problemas de SSO (SSO) baseado em senha
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
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709489"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Solucionar problemas de SSO (SSO) baseado em senha

Para saber os fundamentos do SSO baseado em senha, consulte Autenticação baseada em [senha com o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurar o SSO baseado em senha**

1. [Configurar o](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) login único baseado em senha - Este artigo entra em mais detalhes sobre a opção SSO baseada em senha. Se o aplicativo que você está adicionando requer configuração personalizada e você precisa usar SSO baseado em senha, este artigo é para você.
2. Configurar o login único baseado em senha para aplicativos [in-prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - O Proxy de Aplicativo dá suporte a vários modos de login único. O login baseado em senha destina-se a aplicativos que usam uma combinação de nome de usuário/senha para autenticação. Quando você configura o logom baseado em senha para seu aplicativo, os usuários têm que entrar no aplicativo local uma vez. Depois disso, o Azure Active Directory armazena as informações de entrada e as fornece automaticamente ao aplicativo quando seus usuários as acessam remotamente.
    - Você já deve ter publicado e testado seu aplicativo com Proxy de Aplicativo. Caso não seja, siga as etapas em Publicar aplicativos usando o Proxy de Aplicativo do [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) e, em seguida, continue a configuração do SSO baseado em senha para aplicativos no momento.

Para solucionar problemas de SSO baseado em senha, consulte [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)

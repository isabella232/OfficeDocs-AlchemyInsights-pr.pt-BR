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
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="407b1-102">Solucionar problemas de SSO (SSO) baseado em senha</span><span class="sxs-lookup"><span data-stu-id="407b1-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="407b1-103">Para saber os fundamentos do SSO baseado em senha, consulte Autenticação baseada em [senha com o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="407b1-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="407b1-104">**Configurar o SSO baseado em senha**</span><span class="sxs-lookup"><span data-stu-id="407b1-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="407b1-105">[Configurar o](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) login único baseado em senha - Este artigo entra em mais detalhes sobre a opção SSO baseada em senha.</span><span class="sxs-lookup"><span data-stu-id="407b1-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="407b1-106">Se o aplicativo que você está adicionando requer configuração personalizada e você precisa usar SSO baseado em senha, este artigo é para você.</span><span class="sxs-lookup"><span data-stu-id="407b1-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="407b1-107">Configurar o login único baseado em senha para aplicativos [in-prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - O Proxy de Aplicativo dá suporte a vários modos de login único.</span><span class="sxs-lookup"><span data-stu-id="407b1-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="407b1-108">O login baseado em senha destina-se a aplicativos que usam uma combinação de nome de usuário/senha para autenticação.</span><span class="sxs-lookup"><span data-stu-id="407b1-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="407b1-109">Quando você configura o logom baseado em senha para seu aplicativo, os usuários têm que entrar no aplicativo local uma vez.</span><span class="sxs-lookup"><span data-stu-id="407b1-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="407b1-110">Depois disso, o Azure Active Directory armazena as informações de entrada e as fornece automaticamente ao aplicativo quando seus usuários as acessam remotamente.</span><span class="sxs-lookup"><span data-stu-id="407b1-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="407b1-111">Você já deve ter publicado e testado seu aplicativo com Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="407b1-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="407b1-112">Caso não seja, siga as etapas em Publicar aplicativos usando o Proxy de Aplicativo do [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) e, em seguida, continue a configuração do SSO baseado em senha para aplicativos no momento.</span><span class="sxs-lookup"><span data-stu-id="407b1-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="407b1-113">Para solucionar problemas de SSO baseado em senha, consulte [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="407b1-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>

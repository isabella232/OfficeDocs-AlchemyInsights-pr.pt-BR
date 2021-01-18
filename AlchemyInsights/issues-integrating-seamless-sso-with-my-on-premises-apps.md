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
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="397af-102">Problemas com a integração do SSO Contínuo com meus aplicativos locais</span><span class="sxs-lookup"><span data-stu-id="397af-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="397af-103">Para solucionar problemas com a integração do SSO Contínuo com aplicativos locais, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="397af-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="397af-104">**Etapas recomendadas**</span><span class="sxs-lookup"><span data-stu-id="397af-104">**Recommended steps**</span></span>

1. <span data-ttu-id="397af-105">Para configurar um **aplicativo local** para o single **sign-on** por meio do Proxy de Aplicativo, consulte Cofre de senhas para o single [sign-on com o Proxy de Aplicativo.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)</span><span class="sxs-lookup"><span data-stu-id="397af-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="397af-106">**Solução** de problemas do Proxy de Aplicativo: recomendamos que você comece a analisar o fluxo de solução de problemas, [depurar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemas do Conector de Proxy de Aplicativo para determinar se os conectores de Proxy de Aplicativo estão configurados corretamente.</span><span class="sxs-lookup"><span data-stu-id="397af-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="397af-107">Se você ainda estiver tendo problemas para se conectar ao aplicativo, siga as etapas de solução de problemas em [Depurar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)problemas de aplicativo proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="397af-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="397af-108">Você pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) usando as seguintes ferramentas de depuração do navegador:</span><span class="sxs-lookup"><span data-stu-id="397af-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="397af-109">Iniciar o navegador e navegar até o aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="397af-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="397af-110">Pressione **F12** para abrir o console de depuração.</span><span class="sxs-lookup"><span data-stu-id="397af-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="397af-111">Tente reproduzir a transação e revise a mensagem do console.</span><span class="sxs-lookup"><span data-stu-id="397af-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="397af-112">Uma violação do CORS produz um erro de console sobre a origem.</span><span class="sxs-lookup"><span data-stu-id="397af-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="397af-113">Alguns problemas de CORS não podem ser resolvidos, como quando seu aplicativo redireciona para login.microsoftonline.com autenticar e o token de acesso expira.</span><span class="sxs-lookup"><span data-stu-id="397af-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="397af-114">Em seguida, a chamada CORS falha.</span><span class="sxs-lookup"><span data-stu-id="397af-114">The CORS call then fails.</span></span> <span data-ttu-id="397af-115">Uma solução alternativa para esse cenário é estender o tempo de vida do token de acesso, para evitar que ele expire durante a sessão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="397af-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="397af-116">Para obter mais informações sobre como fazer isso, consulte Tempo de vida [de token configurável na Plataforma de Identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="397af-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="397af-117">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="397af-117">**Recommended documents**</span></span>

- [<span data-ttu-id="397af-118">Como configurar o single sign-on para um aplicativo proxy de aplicativo</span><span class="sxs-lookup"><span data-stu-id="397af-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="397af-119">SAML single sign-on for on-premises applications with Application Proxy</span><span class="sxs-lookup"><span data-stu-id="397af-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="397af-120">Entender e resolver problemas de CORS do Proxy de Aplicativo do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="397af-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="397af-121">Solucionar problemas de configurações de delegação restrita de Kerberos para Proxy de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="397af-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
---
title: Configuração do Proxy de Aplicativo
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876528"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="98279-102">Configuração do Proxy de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98279-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="98279-103">Para entender como configurar um aplicativo proxy de aplicativo no Azure AD para expor seus aplicativos locais à nuvem, consulte Como configurar um aplicativo [proxy de aplicativo.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="98279-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="98279-104">O SSO (single sign-on) permite que os usuários acessem um aplicativo sem autenticar várias vezes.</span><span class="sxs-lookup"><span data-stu-id="98279-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="98279-105">Ele permite que a autenticação única ocorra na nuvem, no Azure Active Directory, e permite que o serviço ou o Conector represente o usuário para concluir quaisquer desafios de autenticação adicionais do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98279-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="98279-106">Para saber mais, consulte [Como configurar o single sign-on para um aplicativo proxy de aplicativo.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)</span><span class="sxs-lookup"><span data-stu-id="98279-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="98279-107">Use [este artigo para](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) solucionar problemas comuns que as pessoas enfrentam ao criar um novo aplicativo proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98279-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="98279-108">Se você estiver tendo um problema ao configurar a autenticação de back-end em seu aplicativo, talvez seja necessário solucionar problemas de configurações de delegação restrita de [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) para o Proxy de Aplicativo ou siga as orientações sobre como configurar o aplicativo com [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) para resolver o problema.</span><span class="sxs-lookup"><span data-stu-id="98279-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>

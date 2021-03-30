---
title: Solucionar problemas de junção do Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403776"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="320dd-102">Solucionar problemas de junção do Azure AD</span><span class="sxs-lookup"><span data-stu-id="320dd-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="320dd-103">Se você estiver configurando registros de dispositivo pela primeira vez, verifique se você analisou Introdução ao gerenciamento de dispositivos no [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) que o orientará sobre como obter dispositivos sob o controle para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="320dd-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="320dd-104">Se você estiver registrando dispositivos no Azure AD diretamente e registrando-os no Intune, você [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) precisará garantir que configurou o [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) e ter o licenciamento em vigor primeiro.</span><span class="sxs-lookup"><span data-stu-id="320dd-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="320dd-105">Verifique se você está autorizado a executar operações no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="320dd-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="320dd-106">Somente um administrador global no Azure AD pode gerenciar configurações para registros de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="320dd-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="320dd-107">Para fazer a implementação de ingressar no Azure AD, consulte [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="320dd-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="320dd-108">Para obter mais detalhes sobre como resolver problemas comuns com a entrada do Azure AD, consulte Perguntas frequentes sobre o [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) e para o dispositivo windows 10 pro, consulte [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span><span class="sxs-lookup"><span data-stu-id="320dd-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>

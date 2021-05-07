---
title: Implantando os complementos para Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233501"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="ff447-102">Implantando os complementos para Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="ff447-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="ff447-103">A Implantação Centralizada é a maneira recomendada de implantar Office de usuários e grupos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ff447-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="ff447-104">Para implantar os complementos, siga as etapas abaixo:</span><span class="sxs-lookup"><span data-stu-id="ff447-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="ff447-105">**Observação:** Para instalar os Office como um usuário individual, consulte Exibir, gerenciar e instalar os [Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="ff447-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="ff447-106">Além disso, certifique-se de que a aquisição individual de Office de complementos da Loja está habilitada.</span><span class="sxs-lookup"><span data-stu-id="ff447-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="ff447-107">Para obter detalhes, consulte [Prevent add-in downloads by off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span><span class="sxs-lookup"><span data-stu-id="ff447-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="ff447-108">Verifique se seu ambiente atende aos requisitos de implantação de complementos usando a Implantação Centralizada.</span><span class="sxs-lookup"><span data-stu-id="ff447-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="ff447-109">Para obter detalhes, consulte [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="ff447-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="ff447-110">Vá para **Configurações**  >  **Aplicativos Integrados** Obter aplicativos no centro de administração  >   Microsoft 365 para implantar os complementos.</span><span class="sxs-lookup"><span data-stu-id="ff447-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="ff447-111">Observações:</span><span class="sxs-lookup"><span data-stu-id="ff447-111">Notes:</span></span> 

- <span data-ttu-id="ff447-112">Os aplicativos integrados exigem que o administrador tenha permissões de Administrador Global ou Exchange Administrador.</span><span class="sxs-lookup"><span data-stu-id="ff447-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="ff447-113">Ao implantar os complementos em vários usuários, recomendamos fazer atribuições usando grupos em vez de usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="ff447-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="ff447-114">Para obter detalhes, consulte Considerações ao atribuir um [complemento a usuários e grupos.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="ff447-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="ff447-115">A Implantação Centralizada não dá suporte a usuários em grupos ou grupos aninhados que têm grupos pai.</span><span class="sxs-lookup"><span data-stu-id="ff447-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="ff447-116">Para obter detalhes, consulte [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="ff447-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="ff447-117">Verifique se o Microsoft 365 Serviço de Gerenciamento de Aplicativos (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') está habilitado para os usuários entrarem.</span><span class="sxs-lookup"><span data-stu-id="ff447-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="ff447-118">Para obter detalhes, consulte [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="ff447-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="ff447-119">Se você tiver problemas ao implantar os complementos usando Aplicativos Integrados, tente implantar usando [Os Complementos](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="ff447-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="ff447-120">Para saber mais, veja:</span><span class="sxs-lookup"><span data-stu-id="ff447-120">For more information, see:</span></span>

<span data-ttu-id="ff447-121">[Implantar os complementos no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gerenciar os complementos no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Usar os cmdlets do PowerShell de Implantação Centralizada para gerenciar os complementos](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicar Office-ins usando a Implantação Centralizada por meio do Microsoft 365 de administração](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Solução de problemas: o usuário não está](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) vendo os complementos 
 [Solucionar erros de usuário com Office Desem seguida](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="ff447-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>
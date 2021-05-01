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
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/30/2021
ms.locfileid: "52107493"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="0332c-102">Implantando os complementos para Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="0332c-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="0332c-103">A Implantação Centralizada é a maneira recomendada de implantar Office de usuários e grupos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="0332c-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="0332c-104">Para implantar os complementos, siga as etapas abaixo:</span><span class="sxs-lookup"><span data-stu-id="0332c-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="0332c-105">**Observação:** Para instalar os Office como um usuário individual, consulte Exibir, gerenciar e instalar os [Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="0332c-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="0332c-106">Além disso, certifique-se de que a aquisição individual de Office de complementos da Loja está habilitada.</span><span class="sxs-lookup"><span data-stu-id="0332c-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="0332c-107">Verifique se seu ambiente atende aos requisitos de implantação de complementos usando a Implantação Centralizada.</span><span class="sxs-lookup"><span data-stu-id="0332c-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="0332c-108">Para obter detalhes, consulte [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="0332c-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="0332c-109">Vá para **Configurações**  >  **Aplicativos Integrados** Obter aplicativos no centro de administração  >   Microsoft 365 para implantar os complementos.</span><span class="sxs-lookup"><span data-stu-id="0332c-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="0332c-110">Observações:</span><span class="sxs-lookup"><span data-stu-id="0332c-110">Notes:</span></span> 

- <span data-ttu-id="0332c-111">Os aplicativos integrados exigem que o administrador tenha permissões de Administrador Global ou Exchange Administrador.</span><span class="sxs-lookup"><span data-stu-id="0332c-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="0332c-112">Ao implantar os complementos em vários usuários, recomendamos fazer atribuições usando grupos em vez de usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="0332c-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="0332c-113">Para obter detalhes, consulte Considerações ao atribuir um [complemento a usuários e grupos.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="0332c-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="0332c-114">A Implantação Centralizada não dá suporte a usuários em grupos ou grupos aninhados que têm grupos pai.</span><span class="sxs-lookup"><span data-stu-id="0332c-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="0332c-115">Para obter detalhes, consulte [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="0332c-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="0332c-116">Verifique se o Microsoft 365 Serviço de Gerenciamento de Aplicativos (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') está habilitado para os usuários entrarem.</span><span class="sxs-lookup"><span data-stu-id="0332c-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="0332c-117">Para obter detalhes, consulte [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="0332c-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="0332c-118">Se você tiver problemas ao implantar os complementos usando Aplicativos Integrados, tente implantar usando [Os Complementos](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="0332c-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="0332c-119">Para mais informações, confira:</span><span class="sxs-lookup"><span data-stu-id="0332c-119">For more information, see:</span></span>

<span data-ttu-id="0332c-120">[Implantar os complementos no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gerenciar os complementos no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Usar os cmdlets do PowerShell de Implantação Centralizada para gerenciar os complementos](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicar Office-ins usando a Implantação Centralizada por meio do Microsoft 365 de administração](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Solução de problemas: o usuário não está](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) vendo os complementos 
 [Solucionar erros de usuário com Office Desem seguida](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="0332c-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>
---
title: Adicionar um grupo a um site do SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582799"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="f4d16-102">Problemas durante a criação de um site conectado ao grupo no SharePoint</span><span class="sxs-lookup"><span data-stu-id="f4d16-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="f4d16-103">Alguns problemas comuns encontrados durante a criação ou recriação de um site conectado ao grupo.</span><span class="sxs-lookup"><span data-stu-id="f4d16-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="f4d16-104">Se você excluiu um grupo e seu site conectado e deseja criar outro site com a mesma URL, será necessário remover permanentemente o site anterior.</span><span class="sxs-lookup"><span data-stu-id="f4d16-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="f4d16-105">Baixe o [Shell de gerenciamento do SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="f4d16-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="f4d16-106">Para obter mais informações sobre como começar a usar o PowerShell, confira [introdução ao Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="f4d16-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="f4d16-107">Remova o site de sites excluídos usando o cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f4d16-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="f4d16-108">O PowerShell é necessário para excluir permanentemente sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="f4d16-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="f4d16-109">Se você estiver criando um site conectado ao grupo e receber um aviso: **outro grupo com o mesmo alias já existe**, verifique os grupos existentes no [centro de administração do Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="f4d16-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="f4d16-110">Para resolver o problema, exclua o grupo existente se ele não for mais necessário ou crie o site com um alias diferente atribuído.</span><span class="sxs-lookup"><span data-stu-id="f4d16-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="f4d16-111">Há diferentes maneiras de criar e usar grupos modernos com o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f4d16-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="f4d16-112">Você pode conectar sites existentes a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f4d16-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="f4d16-113">Para obter mais informações, consulte [Connect a Microsoft 365 Group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="f4d16-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="f4d16-114">Para criar um site conectado ao grupo do Microsoft 365, você precisará criar um [site de equipe](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="f4d16-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>

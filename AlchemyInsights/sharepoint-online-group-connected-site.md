---
title: Adicionar um grupo a um site do SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750508"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="efa17-102">Problemas ao criar ou agrupar sites conectados no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="efa17-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="efa17-103">Há alguns problemas comuns encontrados durante a criação ou recriação de um site conectado ao grupo.</span><span class="sxs-lookup"><span data-stu-id="efa17-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="efa17-104">Se você excluiu um grupo e seu site conectado e deseja criar outro site com a mesma URL, será necessário remover permanentemente o site anterior.</span><span class="sxs-lookup"><span data-stu-id="efa17-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="efa17-105">Baixe o [Shell de gerenciamento do SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="efa17-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="efa17-106">Para saber mais sobre como começar a usar o PowerShell, confira [introdução ao Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="efa17-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="efa17-107">Remova o site de sites excluídos usando o cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="efa17-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="efa17-108">Se você estiver criando um site conectado ao grupo e receber um aviso outro grupo com o mesmo alias já existe, verifique os grupos existentes do [Office 365 a partir do centro de administração](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="efa17-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="efa17-109">Para resolver o problema, exclua o grupo existente se ele não for mais necessário ou crie o site com um alias diferente atribuído.</span><span class="sxs-lookup"><span data-stu-id="efa17-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="efa17-110">Há diferentes maneiras de criar e usar grupos modernos com o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="efa17-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="efa17-111">Você pode conectar sites existentes a um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="efa17-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="efa17-112">Para obter mais informações, consulte [Connect an Office 365 Group using the SharePoint User ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="efa17-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="efa17-113">Para criar um site conectado ao grupo do Office 365, você precisará criar um site de equipe.</span><span class="sxs-lookup"><span data-stu-id="efa17-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="efa17-114">Para obter mais informações, consulte [criar um site de equipe no SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="efa17-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>


---
title: Criar um site do SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786553"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="b238a-102">Criar um site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="b238a-102">Create a SharePoint site</span></span>

<span data-ttu-id="b238a-103">Criar ou gerenciar sites de [sites ativos](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) no centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b238a-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="b238a-104">Para saber mais, confira [gerenciar sites no novo centro de administração do SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="b238a-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="b238a-105">Sobre</span><span class="sxs-lookup"><span data-stu-id="b238a-105">Tips:</span></span>

- <span data-ttu-id="b238a-106">**Não é possível** criar um site com a mesma URL de um site existente.</span><span class="sxs-lookup"><span data-stu-id="b238a-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="b238a-107">Se você excluiu um site e deseja usar novamente a URL, é possível que o site excluído ainda exista em [sites excluídos](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="b238a-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="b238a-108">O site precisará ser excluído permanentemente para reutilizar a URL.</span><span class="sxs-lookup"><span data-stu-id="b238a-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="b238a-109">Para remover completamente um site com PowerShell, consulte o exemplo do cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="b238a-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="b238a-110">Alguns usuários podem não conseguir criar um site.</span><span class="sxs-lookup"><span data-stu-id="b238a-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="b238a-111">[Confira gerenciar a criação de sites no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="b238a-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="b238a-112">É possível que o site pareça estar preso na **criação** de mais tempo do que o esperado.</span><span class="sxs-lookup"><span data-stu-id="b238a-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="b238a-113">Se passar mais de 24 horas desde que você viu o problema pela primeira vez, registre um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="b238a-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b238a-114">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="b238a-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b238a-115">Aguarde pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="b238a-115">Please give us at least 24 hours to complete a solution.</span></span>

---
title: Excluir permanentemente um site no SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771709"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="83405-102">Excluir permanentemente um site no SharePoint</span><span class="sxs-lookup"><span data-stu-id="83405-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="83405-103">Para reutilizar uma URL de um site excluído (para recriar um site) ou excluir um site permanentemente porque ele não é mais usado, você pode usar **Excluir permanentemente** do novo Centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="83405-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="83405-104">Vá para a [página Sites excluídos do novo centro de administração do SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) e entre com uma conta que tenha permissões de administrador para sua organização.</span><span class="sxs-lookup"><span data-stu-id="83405-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="83405-105">Na coluna da esquerda, selecione um site.</span><span class="sxs-lookup"><span data-stu-id="83405-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="83405-106">Clique em **Excluir permanentemente.**.</span><span class="sxs-lookup"><span data-stu-id="83405-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="83405-107">**Observação**: os sites conectados ao grupo não podem ser excluídos permanentemente do Novo Centro de Administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="83405-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="83405-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) precisará ser usado no lugar.</span><span class="sxs-lookup"><span data-stu-id="83405-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="83405-109">Para obter mais informações, consulte [Excluir permanentemente um site.](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="83405-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 

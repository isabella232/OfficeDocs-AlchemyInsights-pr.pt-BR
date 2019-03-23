---
title: Restaurar um conjunto de sites excluído
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753774"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="09977-102">Restaurar um conjunto de sites excluído</span><span class="sxs-lookup"><span data-stu-id="09977-102">Restore a deleted site collection</span></span>

<span data-ttu-id="09977-103">Quando um administrador exclui um conjunto de sites clássico, ele é colocado na lixeira do conjunto de sites, onde é mantido por 93 dias antes de ser excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="09977-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="09977-104">Para restaurar o conjunto de sites:</span><span class="sxs-lookup"><span data-stu-id="09977-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="09977-105">No centro de administração do SharePoint clássico, clique em **Lixeira** na faixa de opções.</span><span class="sxs-lookup"><span data-stu-id="09977-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="09977-106">Marque a caixa de seleção ao lado do conjunto de sites que você deseja restaurar.</span><span class="sxs-lookup"><span data-stu-id="09977-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="09977-107">Clique em **restaurar itens excluídos**.</span><span class="sxs-lookup"><span data-stu-id="09977-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="09977-108">Para restaurar um site de comunicação excluído, você pode usar a nova visualização do centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="09977-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="09977-109">Caso contrário, você precisará usar o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="09977-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="09977-110">Para restaurar um site que pertença a um grupo do Office 365, você precisa restaurar o grupo no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="09977-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="09977-111">Os grupos podem ser restaurados por 30 dias após serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="09977-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


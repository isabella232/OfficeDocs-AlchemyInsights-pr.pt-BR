---
title: Restaure um site excluído
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582223"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="047d4-102">Restaure um site excluído</span><span class="sxs-lookup"><span data-stu-id="047d4-102">Restore a deleted site</span></span>

<span data-ttu-id="047d4-103">Quando um administrador exclui um site do SharePoint, ele é colocado na lixeira do conjunto de sites, onde é mantido por 93 dias antes de ser excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="047d4-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="047d4-104">Para restaurar o site:</span><span class="sxs-lookup"><span data-stu-id="047d4-104">To restore the site:</span></span>
  
1. <span data-ttu-id="047d4-105">No novo centro de administração do SharePoint, clique em **Lixeira** na faixa de opções.</span><span class="sxs-lookup"><span data-stu-id="047d4-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="047d4-106">Marque a caixa de seleção ao lado do conjunto de sites que você deseja restaurar.</span><span class="sxs-lookup"><span data-stu-id="047d4-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="047d4-107">Clique em **restaurar itens excluídos**.</span><span class="sxs-lookup"><span data-stu-id="047d4-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="047d4-108">Para restaurar um site de comunicação excluído, você pode usar o novo centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="047d4-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="047d4-109">Caso contrário, você precisará usar o Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="047d4-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="047d4-110">Para restaurar um site que pertença a um grupo do Microsoft 365, você precisa restaurar o grupo no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="047d4-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="047d4-111">Os grupos podem ser restaurados por 30 dias após serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="047d4-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


---
title: Restaurar um conjunto de sites excluído
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456659"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="f11fd-102">Restaurar um conjunto de sites excluído</span><span class="sxs-lookup"><span data-stu-id="f11fd-102">Restore a deleted site collection</span></span>

<span data-ttu-id="f11fd-p101">Quando um administrador exclui um conjunto de sites clássico, ele é colocado no conjunto de sites Recycle Bin, onde ele é mantido por 93 dias antes de serem excluídos permanentemente. Para restaurar o conjunto de sites:</span><span class="sxs-lookup"><span data-stu-id="f11fd-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="f11fd-105">No Centro de administração do SharePoint clássico, clique em **Lixeira** na faixa de opções.</span><span class="sxs-lookup"><span data-stu-id="f11fd-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="f11fd-106">Marque a caixa de seleção ao lado do conjunto de sites que você deseja restaurar.</span><span class="sxs-lookup"><span data-stu-id="f11fd-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="f11fd-107">Clique em **restaurar itens excluídos**.</span><span class="sxs-lookup"><span data-stu-id="f11fd-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="f11fd-p102">Para restaurar um site excluído de comunicação, você pode usar a guia novo SharePoint admin center preview. Caso contrário, você precisará usar o PowerShell. Para restaurar um site que pertence a um grupo do Office 365, você precisa restaurar o grupo no Centro de administração do Exchange. Grupos podem ser restaurados por 30 dias após sendo excluído.</span><span class="sxs-lookup"><span data-stu-id="f11fd-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  


---
title: Restaure um site excluído
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768536"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="85333-102">Restaure um site excluído</span><span class="sxs-lookup"><span data-stu-id="85333-102">Restore a deleted site</span></span>

<span data-ttu-id="85333-103">Quando um administrador exclui um site do SharePoint, ele é colocado na lixeira do conjunto de sites, onde é mantido por 93 dias antes de ser excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="85333-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="85333-104">Para restaurar o site:</span><span class="sxs-lookup"><span data-stu-id="85333-104">To restore the site:</span></span>
  
1. <span data-ttu-id="85333-105">No novo centro de administração do SharePoint, clique em **Lixeira** na faixa de opções.</span><span class="sxs-lookup"><span data-stu-id="85333-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="85333-106">Marque a caixa de seleção ao lado do conjunto de sites que você deseja restaurar.</span><span class="sxs-lookup"><span data-stu-id="85333-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="85333-107">Clique em **restaurar itens excluídos**.</span><span class="sxs-lookup"><span data-stu-id="85333-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="85333-108">Para restaurar um site de comunicação excluído, você pode usar o novo centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="85333-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="85333-109">Caso contrário, você precisará usar o Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="85333-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="85333-110">Para restaurar um site que pertença a um grupo do Office 365, você precisa restaurar o grupo no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="85333-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="85333-111">Os grupos podem ser restaurados por 30 dias após serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="85333-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


---
title: Restaure um site excluído
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692031"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="292b0-102">Restaure um site excluído</span><span class="sxs-lookup"><span data-stu-id="292b0-102">Restore a deleted site</span></span>

<span data-ttu-id="292b0-103">Quando um administrador exclui um site do SharePoint, ele é colocado na lixeira do conjunto de sites, onde é mantido por 93 dias antes de ser excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="292b0-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="292b0-104">Para restaurar o site:</span><span class="sxs-lookup"><span data-stu-id="292b0-104">To restore the site:</span></span>
  
1. <span data-ttu-id="292b0-105">No novo centro de administração do SharePoint, clique em **Lixeira** na faixa de opções.</span><span class="sxs-lookup"><span data-stu-id="292b0-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="292b0-106">Marque a caixa de seleção ao lado do conjunto de sites que você deseja restaurar.</span><span class="sxs-lookup"><span data-stu-id="292b0-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="292b0-107">Clique em **restaurar itens excluídos**.</span><span class="sxs-lookup"><span data-stu-id="292b0-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="292b0-108">Para restaurar um site de comunicação excluído, você pode usar o novo centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="292b0-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="292b0-109">Caso contrário, você precisará usar o Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="292b0-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="292b0-110">Para restaurar um site que pertença a um grupo do Microsoft 365, você precisa restaurar o grupo no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="292b0-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="292b0-111">Os grupos podem ser restaurados por 30 dias após serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="292b0-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


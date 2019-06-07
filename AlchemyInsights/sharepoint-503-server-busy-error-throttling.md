---
title: Limitação do SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761247"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="8ce98-102">Limitação do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8ce98-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="8ce98-103">Os usuários podem receber um erro de servidor 503 está ocupado ao tentar navegar até sites do SharePoint ou do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8ce98-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="8ce98-104">Esse erro pode ser causado pela limitação no serviço do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ce98-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="8ce98-105">SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="8ce98-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="8ce98-106">O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="8ce98-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="8ce98-107">Se você obter limitadas, 99% do tempo é por causa de código personalizado.</span><span class="sxs-lookup"><span data-stu-id="8ce98-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="8ce98-108">Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="8ce98-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="8ce98-109">Se acreditar que esse erro não está relacionado à limitação, você poderá verificar se há manutenção ativa ocorrendo no locatário, navegando até o [centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="8ce98-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="8ce98-110">Por fim, verifique se você está visitando a página [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar se há avisos/incidentes que possam ocorrer.</span><span class="sxs-lookup"><span data-stu-id="8ce98-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


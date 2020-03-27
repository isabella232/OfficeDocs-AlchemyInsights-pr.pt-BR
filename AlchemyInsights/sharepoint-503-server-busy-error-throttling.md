---
title: Limitação do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958706"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="1ab31-102">Limitação do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1ab31-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="1ab31-103">**Importante**: durante esses horários sem precedentes, estamos executando etapas para garantir que o SharePoint Online e os serviços do onedrive permaneçam altamente disponíveis – visite [ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="1ab31-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1ab31-104">**erro de servidor 503 está ocupado**</span><span class="sxs-lookup"><span data-stu-id="1ab31-104">**503 server is busy error**</span></span>

<span data-ttu-id="1ab31-105">Os usuários podem receber um erro de servidor 503 está ocupado ao tentar navegar até sites do SharePoint ou do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1ab31-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="1ab31-106">Esse erro pode ser causado pela limitação no serviço do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1ab31-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="1ab31-107">SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1ab31-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1ab31-108">O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="1ab31-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="1ab31-109">Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="1ab31-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="1ab31-110">Se acreditar que esse erro não está relacionado à limitação, você poderá verificar se há manutenção ativa ocorrendo no locatário, navegando até o [centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="1ab31-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="1ab31-111">Por fim, verifique se você está visitando a página [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar se há avisos/incidentes que possam ocorrer.</span><span class="sxs-lookup"><span data-stu-id="1ab31-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


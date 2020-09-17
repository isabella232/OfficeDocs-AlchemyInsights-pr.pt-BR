---
title: Limitação do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773835"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="828ff-102">Limitação do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="828ff-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="828ff-103">**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="828ff-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="828ff-104">**erro de servidor 503 está ocupado**</span><span class="sxs-lookup"><span data-stu-id="828ff-104">**503 server is busy error**</span></span>

<span data-ttu-id="828ff-105">Os usuários podem receber um erro de servidor 503 está ocupado ao tentar navegar até sites do SharePoint ou do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="828ff-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="828ff-106">Esse erro pode ser causado pela limitação no serviço do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="828ff-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="828ff-107">SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="828ff-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="828ff-108">A limitação limita o número de ações do usuário ou de chamadas simultâneas (por script ou código) a fim de impedir o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="828ff-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="828ff-109">Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="828ff-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="828ff-110">Se acreditar que esse erro não está relacionado à limitação, você poderá verificar se há manutenção ativa ocorrendo no locatário, navegando até o [centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="828ff-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="828ff-111">Por fim, verifique se você está visitando a página [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar se há avisos/incidentes que possam ocorrer.</span><span class="sxs-lookup"><span data-stu-id="828ff-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


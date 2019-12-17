---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068377"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="c1cee-102">SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários</span><span class="sxs-lookup"><span data-stu-id="c1cee-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="c1cee-103">O SharePoint ou o OneDrive podem ser lentos, inacessíveis ou indisponíveis, ou podem exibir serviços indisponíveis ou 503 erros, por vários motivos:</span><span class="sxs-lookup"><span data-stu-id="c1cee-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="c1cee-104">Se seu site do SharePoint ou do OneDrive estiver lento ou atrasado para vários usuários, pode haver um problema de serviço temporário onde os usuários experimentam atrasos intermitentes ou erros de navegação ao acessar sites do SharePoint ou conteúdo do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c1cee-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="c1cee-105">Verifique o [painel de integridade do serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização é afetada.</span><span class="sxs-lookup"><span data-stu-id="c1cee-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="c1cee-106">Os usuários podem receber um erro de *servidor 503 está ocupado* ao tentar navegar até sites do SharePoint ou do onedrive.</span><span class="sxs-lookup"><span data-stu-id="c1cee-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="c1cee-107">Esse erro pode ser causado pela limitação no serviço do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c1cee-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c1cee-108">SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c1cee-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c1cee-109">O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="c1cee-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c1cee-110">Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c1cee-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="c1cee-111">Se você experimentar um desempenho lento com um **site ou uma** página do SharePoint moderno ou **moderna** , use a ferramenta de [diagnóstico de página](https://aka.ms/perftool) para analisar as páginas.</span><span class="sxs-lookup"><span data-stu-id="c1cee-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="c1cee-112">Se você ainda tiver um desempenho mais lento, revise os recursos na parte inferior deste artigo: [introdução ao ajuste de desempenho para o SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="c1cee-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  
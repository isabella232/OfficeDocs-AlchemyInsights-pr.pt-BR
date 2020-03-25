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
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931214"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5b0ac-102">Limitação do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5b0ac-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="5b0ac-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5b0ac-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5b0ac-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5b0ac-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5b0ac-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5b0ac-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5b0ac-109">**erro de servidor 503 está ocupado**</span><span class="sxs-lookup"><span data-stu-id="5b0ac-109">**503 server is busy error**</span></span>

<span data-ttu-id="5b0ac-110">Os usuários podem receber um erro de servidor 503 está ocupado ao tentar navegar até sites do SharePoint ou do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="5b0ac-111">Esse erro pode ser causado pela limitação no serviço do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5b0ac-112">SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5b0ac-113">O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="5b0ac-114">Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5b0ac-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="5b0ac-115">Se acreditar que esse erro não está relacionado à limitação, você poderá verificar se há manutenção ativa ocorrendo no locatário, navegando até o [centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="5b0ac-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="5b0ac-116">Por fim, verifique se você está visitando a página [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar se há avisos/incidentes que possam ocorrer.</span><span class="sxs-lookup"><span data-stu-id="5b0ac-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


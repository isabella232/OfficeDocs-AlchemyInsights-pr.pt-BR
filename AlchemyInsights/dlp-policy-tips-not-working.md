---
title: Dicas de política de DLP que não funcionam
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932574"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="2dbaa-102">Problemas de dica de política DLP</span><span class="sxs-lookup"><span data-stu-id="2dbaa-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="2dbaa-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2dbaa-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2dbaa-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2dbaa-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2dbaa-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2dbaa-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2dbaa-109">**Dicas de política de DLP**</span><span class="sxs-lookup"><span data-stu-id="2dbaa-109">**DLP policy tips**</span></span>

<span data-ttu-id="2dbaa-110">Ao usar **políticas DLP**, os usuários podem ser notificados de uma violação de política com **dicas de política**.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="2dbaa-111">Os administradores podem configurar dicas de política para exibir durante o teste da política de DLP ou quando a política está no modo de imposição total.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="2dbaa-112">Para configurar dicas de política em sua política de DLP no centro de segurança e conformidade no modo de imposição completa, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="2dbaa-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="2dbaa-113">Verifique se as dicas de política foram **habilitadas** na regra DLP usando as etapas [aqui](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="2dbaa-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="2dbaa-114">Verifique se o **conteúdo corresponde** ao que é **necessário** para acionar a regra descrita neste artigo [aqui](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="2dbaa-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="2dbaa-115">As dicas de política são exibidas no OWA e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="2dbaa-116">No entanto, ao usar o **Outlook 2013 ou posterior**, as dicas de política são exibidas apenas em determinadas condições.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="2dbaa-117">Essas condições estão listadas aqui: [condições suportadas para o Outlook 2013 ou posterior para exibir dicas de política](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="2dbaa-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="2dbaa-118">Para obter informações adicionais sobre dicas de política de DLP, consulte: [Mostrar dicas de política para políticas de DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="2dbaa-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  
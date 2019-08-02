---
title: Limite de emails diários excedido. O fluxo de trabalho foi suspenso.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059627"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="241fb-103">Limite de emails diários excedido.</span><span class="sxs-lookup"><span data-stu-id="241fb-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="241fb-104">O fluxo de trabalho foi suspenso.</span><span class="sxs-lookup"><span data-stu-id="241fb-104">Workflow is suspended.</span></span>

<span data-ttu-id="241fb-105">Esse erro pode ser recebido nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="241fb-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="241fb-106">Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho do SharePoint 2010 ou SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="241fb-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="241fb-107">O fluxo de trabalho é configurado para enviar uma mensagem de email personalizada para mais de 200 usuários por vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.</span><span class="sxs-lookup"><span data-stu-id="241fb-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="241fb-108">Quando você executa o fluxo de trabalho, a mensagem de email não é enviada e você observa o seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="241fb-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="241fb-109">Para um fluxo de trabalho usando o tipo de plataforma do SharePoint 2013, navegue até a página **status do fluxo de trabalho** .</span><span class="sxs-lookup"><span data-stu-id="241fb-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="241fb-110">Na página status do fluxo de trabalho, o **status interno** é definido como **iniciado**e o balão de informações exibe **não é possível enviar a um destinatário**.</span><span class="sxs-lookup"><span data-stu-id="241fb-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="241fb-111">Para contornar esse problema, configure seu fluxo de trabalho para enviar mensagens de email sem exceder os limites de remetentes do [Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="241fb-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="241fb-112">Por exemplo, use uma pausa no fluxo de trabalho, envie o email para um grupo do Office 365, um grupo de distribuição ou um grupo de segurança habilitado para email ou envie a mensagem para menos de 200 destinatários por vez.</span><span class="sxs-lookup"><span data-stu-id="241fb-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="241fb-113">Para obter mais informações, consulte o [artigo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)a seguir.</span><span class="sxs-lookup"><span data-stu-id="241fb-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="241fb-114">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="241fb-114">Related topics</span></span>
- [<span data-ttu-id="241fb-115">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="241fb-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="241fb-116">SharePoint e fluxo</span><span class="sxs-lookup"><span data-stu-id="241fb-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
---
title: O fluxo de trabalho não está sendo iniciado
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738077"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="20bac-102">O fluxo de trabalho não está sendo iniciado</span><span class="sxs-lookup"><span data-stu-id="20bac-102">Workflow is not starting</span></span>

- <span data-ttu-id="20bac-103">Os fluxos de trabalho do SharePoint 2010 e do SharePoint 2013 não estão sendo iniciados.</span><span class="sxs-lookup"><span data-stu-id="20bac-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="20bac-104">Se o seu fluxo de trabalho não estiver sendo iniciado, pode haver um problema de serviço temporário no qual os usuários podem enfrentar atrasos intermitentes com o progresso do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="20bac-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="20bac-105">Verifique o [painel de integridade do serviço](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização é afetada.</span><span class="sxs-lookup"><span data-stu-id="20bac-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="20bac-106">Se passar mais de 24 horas desde que você viu o problema pela primeira vez, registre um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="20bac-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="20bac-107">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="20bac-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="20bac-108">Aguarde pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="20bac-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="20bac-109">Fluxos de trabalho do SharePoint 2010 atrasados no início.</span><span class="sxs-lookup"><span data-stu-id="20bac-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="20bac-110">Isso ocorre se o fluxo de trabalho é acionado em lotes grandes.</span><span class="sxs-lookup"><span data-stu-id="20bac-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="20bac-111">(por exemplo, quando vários itens são adicionados ao mesmo tempo).</span><span class="sxs-lookup"><span data-stu-id="20bac-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="20bac-112">Os fluxos de trabalho não são projetados para executar em tempo real, de forma que um atraso é o comportamento de design.</span><span class="sxs-lookup"><span data-stu-id="20bac-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="20bac-113">Se o fluxo de trabalho é um XMOL (Extensible Object Markup Language) complexo, a compilação pode ser lenta.</span><span class="sxs-lookup"><span data-stu-id="20bac-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="20bac-114">Confira [este](https://support.microsoft.com//kb/3043697) artigo.</span><span class="sxs-lookup"><span data-stu-id="20bac-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="20bac-115">Você deve simplificar o fluxo de trabalho ou recriá-lo usando o tipo de plataforma de fluxo de trabalho do Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="20bac-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="20bac-116">Se o histórico do seu fluxo de trabalho tiver crescido grande, talvez você queira limpar os itens ou criar uma nova lista de histórico.</span><span class="sxs-lookup"><span data-stu-id="20bac-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="20bac-117">Mais informações: [Limpar histórico de fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="20bac-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="20bac-118">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="20bac-118">Related topics</span></span>
<span data-ttu-id="20bac-119">Deseja experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="20bac-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="20bac-120">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="20bac-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="20bac-121">SharePoint e fluxo</span><span class="sxs-lookup"><span data-stu-id="20bac-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



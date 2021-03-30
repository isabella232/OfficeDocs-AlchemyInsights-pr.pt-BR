---
title: O fluxo de trabalho não está iniciando
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403731"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="7a39a-102">O fluxo de trabalho não está iniciando</span><span class="sxs-lookup"><span data-stu-id="7a39a-102">Workflow is not starting</span></span>

- <span data-ttu-id="7a39a-103">Os fluxos de trabalho do SharePoint 2010 e do SharePoint 2013 não estão iniciando.</span><span class="sxs-lookup"><span data-stu-id="7a39a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="7a39a-104">Se o fluxo de trabalho não estiver iniciando, pode haver um problema de serviço temporário em que os usuários possam ter atrasos intermitentes com o andamento do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7a39a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="7a39a-105">Verifique o [Painel de Saúde do Serviço](https://admin.microsoft.com/AdminPortal/Home/servicehealth) para ver se sua organização está impactada.</span><span class="sxs-lookup"><span data-stu-id="7a39a-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="7a39a-106">Se mais de 24 horas se passaram desde que você viu esse problema pela primeira vez, registre um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="7a39a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7a39a-107">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="7a39a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7a39a-108">Dê-nos pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="7a39a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="7a39a-109">Fluxos de trabalho do SharePoint 2010 atrasados no início.</span><span class="sxs-lookup"><span data-stu-id="7a39a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="7a39a-110">Isso ocorrerá se o fluxo de trabalho for disparado em lotes grandes.</span><span class="sxs-lookup"><span data-stu-id="7a39a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="7a39a-111">(por exemplo, quando vários itens são adicionados ao mesmo tempo).</span><span class="sxs-lookup"><span data-stu-id="7a39a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="7a39a-112">Os fluxos de trabalho não são projetados para ser executados em tempo real, portanto, um atraso é o comportamento de design.</span><span class="sxs-lookup"><span data-stu-id="7a39a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="7a39a-113">Se o Fluxo de Trabalho for XMOL (Linguagem de Marcação de Objeto Extensível complexo), a compilação poderá ser lenta.</span><span class="sxs-lookup"><span data-stu-id="7a39a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="7a39a-114">Confira [este](https://support.microsoft.com//kb/3043697) artigo.</span><span class="sxs-lookup"><span data-stu-id="7a39a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="7a39a-115">Você deve simplificar o fluxo de trabalho ou reprojetá-lo usando o tipo de plataforma de fluxo de trabalho do Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="7a39a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="7a39a-116">Se o histórico do fluxo de trabalho tiver se aumentado, talvez você queira limpar os itens ou criar uma nova lista de histórico.</span><span class="sxs-lookup"><span data-stu-id="7a39a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="7a39a-117">Mais informações : [Limpar Histórico do Fluxo de Trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="7a39a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="7a39a-118">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="7a39a-118">Related topics</span></span>
<span data-ttu-id="7a39a-119">Deseja experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="7a39a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="7a39a-120">Criar Fluxo</span><span class="sxs-lookup"><span data-stu-id="7a39a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7a39a-121">SharePoint e Flow</span><span class="sxs-lookup"><span data-stu-id="7a39a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 

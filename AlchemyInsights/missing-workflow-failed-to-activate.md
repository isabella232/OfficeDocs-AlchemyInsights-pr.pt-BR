---
title: Falta de fluxo de trabalho ao ativar
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418421"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="596be-102">Falta de fluxo de trabalho ao ativar</span><span class="sxs-lookup"><span data-stu-id="596be-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="596be-103">Em um conjunto de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho reutilizável globalmente (como "Approval-SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="596be-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="596be-104">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="596be-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="596be-105">Abra o site raiz do conjunto de sites no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="596be-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="596be-106">Em **objetos de site**, selecione **fluxos de trabalho**.</span><span class="sxs-lookup"><span data-stu-id="596be-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="596be-107">Na **nova** seção da faixa de opções **fluxos de trabalho** , selecione fluxo de trabalho reutilizável. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="596be-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="596be-108">No formulário **criar fluxo de trabalho** reutilizável, insira o nome \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="596be-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="596be-109">Para **tipo de plataforma**, clique em **fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="596be-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="596be-110">Na seção **salvar** da faixa de opções de **fluxo de trabalho** , selecione **publicar**.</span><span class="sxs-lookup"><span data-stu-id="596be-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="596be-111">Na seção **gerenciar** da faixa de opções de **fluxo de trabalho** , selecione **publicar globalmente**.</span><span class="sxs-lookup"><span data-stu-id="596be-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="596be-112">Na caixa de diálogo de confirmação exibida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="596be-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="596be-113">Em um navegador da Web, localize o site raiz do conjunto de sites e acesse os **recursos do conjunto de sites**configurações \> de **site** .</span><span class="sxs-lookup"><span data-stu-id="596be-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="596be-114">Em seguida, alterne o recurso **fluxos de trabalho** :</span><span class="sxs-lookup"><span data-stu-id="596be-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="596be-115">· Se o recurso estiver *ativado* , clique em desativar e, em seguida **,** clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="596be-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="596be-116">· Se o recurso for *desativado* , clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="596be-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="596be-117">Para obter mais informações, consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.</span><span class="sxs-lookup"><span data-stu-id="596be-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


---
title: Não é possível adicionar o fluxo de trabalho de aprovação 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748672"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="77656-102">Não é possível adicionar o fluxo de trabalho de aprovação 2010</span><span class="sxs-lookup"><span data-stu-id="77656-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="77656-103">Em um conjunto de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho reutilizável globalmente (como "Approval-SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="77656-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="77656-104">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="77656-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="77656-105">Abra o site raiz do conjunto de sites no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="77656-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="77656-106">Em **objetos de site**, selecione **fluxos de trabalho**.</span><span class="sxs-lookup"><span data-stu-id="77656-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="77656-107">Na **nova** seção da faixa de opções **fluxos de trabalho** , selecione fluxo de **trabalho reutilizável**.</span><span class="sxs-lookup"><span data-stu-id="77656-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="77656-108">No formulário **criar fluxo de trabalho reutilizável** , insira o nome \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="77656-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="77656-109">Para **tipo de plataforma**, clique em **fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="77656-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="77656-110">Na seção **salvar** da faixa de opções de **fluxo de trabalho** , selecione **publicar**.</span><span class="sxs-lookup"><span data-stu-id="77656-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="77656-111">Na seção **gerenciar** da faixa de opções de **fluxo de trabalho** , selecione **publicar globalmente**.</span><span class="sxs-lookup"><span data-stu-id="77656-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="77656-112">Na caixa de diálogo de confirmação exibida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="77656-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="77656-113">Em um navegador da Web, localize o site raiz do conjunto de sites e acesse os **recursos do conjunto de sites**configurações \> de **site** .</span><span class="sxs-lookup"><span data-stu-id="77656-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="77656-114">Alternar o recurso de **fluxos de trabalho** :</span><span class="sxs-lookup"><span data-stu-id="77656-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="77656-115">· Se o recurso estiver *ativado* , clique em desativar e, em seguida **,** clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="77656-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="77656-116">· Se o recurso for *desativado* , clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="77656-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="77656-117">Para obter mais informações, consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.</span><span class="sxs-lookup"><span data-stu-id="77656-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


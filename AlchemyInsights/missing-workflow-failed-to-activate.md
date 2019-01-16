---
title: Falta de fluxo de trabalho não pôde ser ativado
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275286"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="f84ba-102">Falta de fluxo de trabalho não pôde ser ativado</span><span class="sxs-lookup"><span data-stu-id="f84ba-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="f84ba-103">Em um conjunto de sites do Microsoft SharePoint, é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="f84ba-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f84ba-104">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="f84ba-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f84ba-105">Abra o site raiz do conjunto de sites no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f84ba-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f84ba-106">Em **Objetos de Site**, selecione **fluxos de trabalho**.</span><span class="sxs-lookup"><span data-stu-id="f84ba-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f84ba-107">Na seção **novo** da faixa de opções de **fluxos de trabalho** , selecione o **Fluxo de trabalho reutilizável**.</span><span class="sxs-lookup"><span data-stu-id="f84ba-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f84ba-p101">No formulário **Criar fluxo de trabalho reutilizável** , insira o nome \* \* *Repair2010* \* \*. Para o **Tipo de plataforma**, clique em **Fluxo de trabalho do SharePoint 2010**e clique em **Okey**.</span><span class="sxs-lookup"><span data-stu-id="f84ba-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f84ba-110">Na seção **Salvar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar**.</span><span class="sxs-lookup"><span data-stu-id="f84ba-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f84ba-p102">Na seção **Gerenciar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **Okey**.</span><span class="sxs-lookup"><span data-stu-id="f84ba-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f84ba-p103">Em um navegador da web, localize o site raiz do conjunto de sites e depois acesse **Configurações do Site** \> **Recursos do conjunto de sites**. Em seguida, ativa/desativa o recurso de **fluxos de trabalho** :</span><span class="sxs-lookup"><span data-stu-id="f84ba-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f84ba-115">· Se o recurso está *ativado* , clique em **Desativar** e, em seguida, clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="f84ba-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f84ba-116">· Se o recurso estiver *desativado* , clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="f84ba-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f84ba-117">Para obter mais informações consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.</span><span class="sxs-lookup"><span data-stu-id="f84ba-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


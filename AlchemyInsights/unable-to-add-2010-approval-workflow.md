---
title: Não é possível adicionar o fluxo de trabalho de aprovação de 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925404"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="34b73-102">Não é possível adicionar o fluxo de trabalho de aprovação de 2010</span><span class="sxs-lookup"><span data-stu-id="34b73-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="34b73-103">Em um conjunto de sites do Microsoft SharePoint, é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") a uma lista ou biblioteca.</span><span class="sxs-lookup"><span data-stu-id="34b73-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="34b73-104">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="34b73-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="34b73-105">Abra o site raiz do conjunto de sites no SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="34b73-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="34b73-106">Em **Objetos de Site**, selecione **fluxos de trabalho**.</span><span class="sxs-lookup"><span data-stu-id="34b73-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="34b73-107">Na seção **novo** da faixa de opções de **fluxos de trabalho** , selecione o **Fluxo de trabalho reutilizável**.</span><span class="sxs-lookup"><span data-stu-id="34b73-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="34b73-p101">No formulário **Criar fluxo de trabalho reutilizável** , insira o nome \* \* *Repair2010* \* \*. Para o **Tipo de plataforma**, clique em **Fluxo de trabalho do SharePoint 2010**e clique em **Okey**.</span><span class="sxs-lookup"><span data-stu-id="34b73-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="34b73-110">Na seção **Salvar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar**.</span><span class="sxs-lookup"><span data-stu-id="34b73-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="34b73-p102">Na seção **Gerenciar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **Okey**.</span><span class="sxs-lookup"><span data-stu-id="34b73-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="34b73-p103">Em um navegador da web, localize o site raiz do conjunto de sites e depois acesse **Configurações do Site** \> **Recursos do conjunto de sites**. Ativa/desativa o recurso de **fluxos de trabalho** :</span><span class="sxs-lookup"><span data-stu-id="34b73-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="34b73-115">· Se o recurso está *ativado* , clique em **Desativar** e, em seguida, clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="34b73-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="34b73-116">· Se o recurso estiver *desativado* , clique em **Ativar**.</span><span class="sxs-lookup"><span data-stu-id="34b73-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="34b73-117">Para obter mais informações consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.</span><span class="sxs-lookup"><span data-stu-id="34b73-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


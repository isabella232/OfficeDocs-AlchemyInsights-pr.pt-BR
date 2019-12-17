---
title: Falta de fluxo de trabalho ao ativar
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052601"
---
# <a name="missing-workflow-failed-to-activate"></a>Falta de fluxo de trabalho ao ativar

Em um conjunto de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho reutilizável globalmente (como "Approval-SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver esse problema, siga estas etapas: 
  
1. Abra o site raiz do conjunto de sites no SharePoint Designer 2013.
  
2. Em **objetos de site**, selecione **fluxos de trabalho**. 
  
3. Na **nova** seção da faixa de opções **fluxos de trabalho** , selecione fluxo de **trabalho reutilizável**. 
  
4. No formulário **criar fluxo de trabalho reutilizável** , insira o nome * * *Repair2010* * *. Para **tipo de plataforma**, clique em **fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**. 
  
1. Na seção **salvar** da faixa de opções de **fluxo de trabalho** , selecione **publicar**. 
  
2. Na seção **gerenciar** da faixa de opções de **fluxo de trabalho** , selecione **publicar globalmente**. Na caixa de diálogo de confirmação exibida, selecione **OK**. 
  
3. Em um navegador da Web, localize o site raiz do conjunto de sites e acesse os **recursos do conjunto de sites**configurações \> de **site** . Em seguida, alterne o recurso **fluxos de trabalho** : 
  
· Se o recurso estiver *ativado* , clique em desativar e, em seguida **,** clique em **Ativar**. 
  
· Se o recurso for *desativado* , clique em **Ativar**. 
  
Para obter mais informações, consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.
  


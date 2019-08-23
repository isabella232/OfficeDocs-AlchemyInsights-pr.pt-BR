---
title: Não é possível adicionar o fluxo de trabalho de aprovação 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 1f564c5d1e689dcf41b22fab5a05ab1b488c2b0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558605"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Não é possível adicionar o fluxo de trabalho de aprovação 2010

Em um conjunto de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho reutilizável globalmente (como "Approval-SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver esse problema, siga estas etapas: 
  
1. Abra o site raiz do conjunto de sites no SharePoint Designer 2013.
  
2. Em **objetos de site**, selecione **fluxos de trabalho**. 
  
3. Na **nova** seção da faixa de opções **fluxos de trabalho** , selecione fluxo de trabalho reutilizável. **** 
  
4. No formulário **criar fluxo de trabalho** reutilizável, insira o nome * * *Repair2010* * *. Para **tipo de plataforma**, clique em **fluxo de trabalho do SharePoint 2010**e, em seguida, clique em **OK**. 
  
1. Na seção **salvar** da faixa de opções de **fluxo de trabalho** , selecione **publicar**. 
  
2. Na seção **gerenciar** da faixa de opções de **fluxo de trabalho** , selecione **publicar globalmente**. Na caixa de diálogo de confirmação exibida, selecione **OK**. 
  
3. Em um navegador da Web, localize o site raiz do conjunto de sites e acesse os **recursos do conjunto de sites**configurações \> de **site** . Alternar o recurso de **fluxos de trabalho** : 
  
· Se o recurso estiver *ativado* , clique em desativar e, em seguida **,** clique em **Ativar**. 
  
· Se o recurso for *desativado* , clique em **Ativar**. 
  
Para obter mais informações, consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.
  


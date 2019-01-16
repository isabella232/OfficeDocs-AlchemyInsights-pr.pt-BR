---
title: Não é possível adicionar o fluxo de trabalho de aprovação de 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275427"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Não é possível adicionar o fluxo de trabalho de aprovação de 2010

Em um conjunto de sites do Microsoft SharePoint, é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver esse problema, siga estas etapas: 
  
1. Abra o site raiz do conjunto de sites no SharePoint Designer 2013.
  
2. Em **Objetos de Site**, selecione **fluxos de trabalho**. 
  
3. Na seção **novo** da faixa de opções de **fluxos de trabalho** , selecione o **Fluxo de trabalho reutilizável**. 
  
4. No formulário **Criar fluxo de trabalho reutilizável** , insira o nome * * *Repair2010* * *. Para o **Tipo de plataforma**, clique em **Fluxo de trabalho do SharePoint 2010**e clique em **Okey**. 
  
1. Na seção **Salvar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar**. 
  
2. Na seção **Gerenciar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **Okey**. 
  
3. Em um navegador da web, localize o site raiz do conjunto de sites e depois acesse **Configurações do Site** \> **Recursos do conjunto de sites**. Ativa/desativa o recurso de **fluxos de trabalho** : 
  
· Se o recurso está *ativado* , clique em **Desativar** e, em seguida, clique em **Ativar**. 
  
· Se o recurso estiver *desativado* , clique em **Ativar**. 
  
Para obter mais informações consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.
  


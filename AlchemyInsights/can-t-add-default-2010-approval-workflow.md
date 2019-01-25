---
title: Não é possível adicionar padrão fluxo de trabalho de aprovação de 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456647"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Não é possível adicionar padrão fluxo de trabalho de aprovação de 2010

Em um conjunto de sites do Microsoft SharePoint, é possível adicionar um fluxo de trabalho reutilizável globalmente (por exemplo, "aprovação - SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver esse problema, siga estas etapas: 
  
1. Abra o site raiz do conjunto de sites no SharePoint Designer 2013.
  
2. Em **Objetos de Site**, selecione **fluxos de trabalho**. 
  
3. Na seção **novo** da faixa de opções de **fluxos de trabalho** , selecione o **Fluxo de trabalho reutilizável**. 
  
4. No formulário **Criar fluxo de trabalho reutilizável** , insira o nome * **Repair2010***. Para o **Tipo de plataforma**, selecione **o fluxo de trabalho do SharePoint 2010**e selecione **Okey**. 
  
5. Na seção **Salvar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar**. 
  
6. Na seção **Gerenciar** da faixa de opções do **fluxo de trabalho** , selecione **Publicar globalmente**. Na caixa de diálogo de confirmação que aparece, selecione **Okey**. 
  
7. Em um navegador da web, localize o site raiz do conjunto de sites e depois acesse **Configurações do Site** \> **Recursos do conjunto de sites**. Em seguida, ativa/desativa o recurso de **fluxos de trabalho** : 
  
· Se o recurso está *ativado* , clique em **Desativar** e, em seguida, clique em **Ativar**. 
  
· Se o recurso estiver *desativado* , clique em **Ativar**. 
  
Para obter mais informações consulte o [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)a seguir.
  


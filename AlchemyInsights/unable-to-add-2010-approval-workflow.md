---
title: Não é possível adicionar o Fluxo de Trabalho de Aprovação 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020324"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Não é possível adicionar o Fluxo de Trabalho de Aprovação 2010

Em um conjunto de sites do Microsoft SharePoint, você não pode adicionar um fluxo de trabalho reutilizável globalmente (como "Aprovação - SharePoint 2010") a uma lista ou biblioteca.
  
Para resolver esse problema, siga estas etapas: 
  
1. Abra o site raiz do conjunto de sites no SharePoint Designer 2013.
  
2. Em **Objetos de Site,** selecione **Fluxos de Trabalho**. 
  
3. Na seção **Novo** da faixa de opções **Fluxos de** Trabalho, selecione **Fluxo de Trabalho Reutilizável**. 
  
4. No formulário **Criar Fluxo de Trabalho Reutilizável,** digite o nome ** *Repair2010* **. Para **Tipo de Plataforma,** clique SharePoint Fluxo de **Trabalho 2010** e clique em **OK**. 
  
1. Na seção **Salvar** da faixa de opções **fluxo de** trabalho, selecione **Publicar**. 
  
2. Na seção **Gerenciar** da faixa de opções **fluxo de** trabalho, selecione **Publicar Globalmente**. Na caixa de diálogo de confirmação exibida, selecione **OK**. 
  
3. Em um navegador da Web, localize o site raiz do conjunto de sites e, em seguida, acesse **Site Configurações** Recursos do Conjunto \> **de Sites.** Alterne o **recurso Fluxos de** Trabalho: 
  
· Se o recurso for  *Ativado,*  clique em **Desativar e** clique em **Ativar**. 
  
· Se o recurso for  *Desativado,*  clique em **Ativar**. 
  
Para obter mais informações, consulte o seguinte [artigo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  


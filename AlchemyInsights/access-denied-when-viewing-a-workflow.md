---
title: Acesso negado ao exibir um fluxo de trabalho
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050513"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acesso negado ao exibir um fluxo de trabalho

Os fluxos de trabalho do SharePoint 2013 que tentam enviar um email a um grupo do SharePoint podem falhar com uma mensagem de erro "acesso negado" se a associação do grupo do SharePoint não estiver definida como todos.
  
 **Para resolver esse problema, siga estas etapas:**
  
 1. Permitir que todos vejam os membros do grupo do SharePoint.
  
 2. Remova o grupo do SharePoint da linha para ou CC do email.
  
 3. Adicione explicitamente os usuários à linha para ou CC se a visibilidade da associação não puder ser alterada para o grupo do SharePoint.
  
Para exibir mais detalhes, consulte [http não autorizado para/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  
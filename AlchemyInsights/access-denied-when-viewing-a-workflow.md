---
title: Acesso negado ao visualizar um fluxo de trabalho
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918811"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acesso negado ao visualizar um fluxo de trabalho

SharePoint 2013 fluxos de trabalho que tentam enviar um email para um grupo do SharePoint pode falhar com uma mensagem de erro "Acesso negado" se a associação de grupo do SharePoint não estiver definida como todos.
  
 **Para resolver esse problema, siga estas etapas:**
  
 1. Permitir todas as pessoas ver os membros do grupo do SharePoint. 
  
 2. Remova o grupo do SharePoint para ou CC linha do email. 
  
 3. Adicione explicitamente os usuários para ou CC linha se a visibilidade de associação não pode ser alterada para o grupo do SharePoint. 
  
Para exibir mais detalhes, consultem [HTTP não autorizado para /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  


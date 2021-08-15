---
title: Acesso negado ao exibir um Fluxo de Trabalho
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955189"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acesso negado ao exibir um Fluxo de Trabalho

SharePoint fluxos de trabalho 2013 que tentam enviar um email para um grupo SharePoint podem falhar com uma mensagem de erro "Acesso Negado" se a associação do grupo SharePoint não estiver definida como Todos.
  
 **Para resolver esse problema, faça estas etapas:**
  
 1. Permitir que todos vejam os membros do SharePoint grupo.
  
 2. Remova o SharePoint grupo da linha Para ou CC do email.
  
 3. Adicione explicitamente os usuários à linha Para ou CC se a visibilidade de associação não puder ser alterada para SharePoint grupo.
  
Para exibir mais detalhes, consulte HTTP Não autorizado [para /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  
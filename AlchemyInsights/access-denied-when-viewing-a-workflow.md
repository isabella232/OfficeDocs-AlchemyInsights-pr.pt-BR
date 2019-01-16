---
title: Acesso negado ao visualizar um fluxo de trabalho
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274419"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="c3410-102">Acesso negado ao visualizar um fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="c3410-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="c3410-103">SharePoint 2013 fluxos de trabalho que tentam enviar um email para um grupo do SharePoint pode falhar com uma mensagem de erro "Acesso negado" se a associação de grupo do SharePoint não estiver definida como todos.</span><span class="sxs-lookup"><span data-stu-id="c3410-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="c3410-104">**Para resolver esse problema, siga estas etapas:**</span><span class="sxs-lookup"><span data-stu-id="c3410-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="c3410-105">Permitir todas as pessoas ver os membros do grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c3410-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="c3410-106">Remova o grupo do SharePoint para ou CC linha do email.</span><span class="sxs-lookup"><span data-stu-id="c3410-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="c3410-107">Adicione explicitamente os usuários para ou CC linha se a visibilidade de associação não pode ser alterada para o grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c3410-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="c3410-108">Para exibir mais detalhes, consultem [HTTP não autorizado para /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c3410-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  


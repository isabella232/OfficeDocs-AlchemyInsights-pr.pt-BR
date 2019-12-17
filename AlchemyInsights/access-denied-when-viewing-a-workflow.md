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
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="c2423-102">Acesso negado ao exibir um fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="c2423-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="c2423-103">Os fluxos de trabalho do SharePoint 2013 que tentam enviar um email a um grupo do SharePoint podem falhar com uma mensagem de erro "acesso negado" se a associação do grupo do SharePoint não estiver definida como todos.</span><span class="sxs-lookup"><span data-stu-id="c2423-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="c2423-104">**Para resolver esse problema, siga estas etapas:**</span><span class="sxs-lookup"><span data-stu-id="c2423-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="c2423-105">Permitir que todos vejam os membros do grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c2423-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="c2423-106">Remova o grupo do SharePoint da linha para ou CC do email.</span><span class="sxs-lookup"><span data-stu-id="c2423-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="c2423-107">Adicione explicitamente os usuários à linha para ou CC se a visibilidade da associação não puder ser alterada para o grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c2423-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="c2423-108">Para exibir mais detalhes, consulte [http não autorizado para/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c2423-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  
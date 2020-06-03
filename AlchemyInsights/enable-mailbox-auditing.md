---
title: Habilitar a auditoria de caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506942"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="8b80f-102">Habilitar a auditoria de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="8b80f-102">Enable mailbox auditing</span></span>

<span data-ttu-id="8b80f-103">Para habilitar a auditoria de caixa de correio para um único usuário ou uma organização inteira, os cmdlets a seguir devem ser executados a partir do Shell de energia remoto:</span><span class="sxs-lookup"><span data-stu-id="8b80f-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="8b80f-104">**Único usuário**</span><span class="sxs-lookup"><span data-stu-id="8b80f-104">**Single User**</span></span>
  
<span data-ttu-id="8b80f-105">Set-Mailbox-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="8b80f-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="8b80f-106">**Organização**</span><span class="sxs-lookup"><span data-stu-id="8b80f-106">**Organization**</span></span>
  
<span data-ttu-id="8b80f-107">Get-Mailbox-Results Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="8b80f-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="8b80f-108">Saiba Mais</span><span class="sxs-lookup"><span data-stu-id="8b80f-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  


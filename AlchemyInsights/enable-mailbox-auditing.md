---
title: Habilitar a auditoria de caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736241"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="d8666-102">Habilitar a auditoria de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="d8666-102">Enable mailbox auditing</span></span>

<span data-ttu-id="d8666-103">Para habilitar a auditoria de caixa de correio para um único usuário ou uma organização inteira, os cmdlets a seguir devem ser executados a partir do Shell de energia remoto:</span><span class="sxs-lookup"><span data-stu-id="d8666-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="d8666-104">**Único usuário**</span><span class="sxs-lookup"><span data-stu-id="d8666-104">**Single User**</span></span>
  
<span data-ttu-id="d8666-105">Set-Mailbox-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d8666-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="d8666-106">**Organização**</span><span class="sxs-lookup"><span data-stu-id="d8666-106">**Organization**</span></span>
  
<span data-ttu-id="d8666-107">Get-Mailbox-Results Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d8666-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="d8666-108">Saiba mais</span><span class="sxs-lookup"><span data-stu-id="d8666-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  


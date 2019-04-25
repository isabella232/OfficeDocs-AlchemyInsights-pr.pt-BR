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
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403735"
---
# <a name="enable-mailbox-auditing"></a>Habilitar a auditoria de caixa de correio

Para habilitar a auditoria de caixa de correio para um único usuário ou uma organização inteira, os cmdlets a seguir devem ser executados a partir do Shell de energia remoto:
  
 **Único usuário**
  
Set-Mailbox-Identity "Jane Dow"-AuditEnabled $true
  
 **Organização**
  
Get-Mailbox-Results unLimited-Filter {RecipientTypeDetails-EQ "userMailbox"} | Set-Mailbox-AuditEnabled $true
  
[Saiba mais](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  


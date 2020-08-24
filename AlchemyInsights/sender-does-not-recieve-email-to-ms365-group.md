---
title: O remetente não recebe email enviado ao grupo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46846047"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>O remetente não recebe email enviado ao grupo Microsoft 365

Por padrão, o remetente de uma mensagem de email para um grupo Microsoft 365 não recebe uma cópia da mensagem em sua caixa de entrada, mesmo que o remetente seja um membro do grupo.

Use este comando EXO PowerShell para permitir que o remetente receba uma cópia de cada email que enviar para o grupo Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Para habilitar a configuração para todas as caixas de correio de uma só vez:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Observação** Alterações feitas nessa configuração levam até uma hora para entrarem em vigor.
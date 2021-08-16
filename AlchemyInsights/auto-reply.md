---
title: 'Para configurar a resposta automática para todos os emails enviados ao grupo do Microsoft 365:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 3ed937d38627c1089c9203550498ce7b21ce01c0c5a2deea7326f8057f5338d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036120"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Para configurar a resposta automática para todos os emails enviados ao grupo do Microsoft 365:

**Conecte-se ao EXO PowerShell usando a conta de administrador do locatário e use o seguinte comando**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> Altere **groupmailbox** para um nome de grupo para o qual deseja configurar a resposta automática.


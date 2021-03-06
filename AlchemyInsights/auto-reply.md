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
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430706"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a><span data-ttu-id="b26a2-102">Para configurar a resposta automática para todos os emails enviados ao grupo do Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="b26a2-102">To configure auto reply for all emails sent to Microsoft 365 group:</span></span>

<span data-ttu-id="b26a2-103">**Conecte-se ao EXO PowerShell usando a conta de administrador do locatário e use o seguinte comando**:</span><span class="sxs-lookup"><span data-stu-id="b26a2-103">**Connect to EXO PowerShell using tenant admin account and use following command**:</span></span>

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> <span data-ttu-id="b26a2-104">Altere **groupmailbox** para um nome de grupo para o qual deseja configurar a resposta automática.</span><span class="sxs-lookup"><span data-stu-id="b26a2-104">Change **groupmailbox** to a group name that you want to configure auto reply on.</span></span>


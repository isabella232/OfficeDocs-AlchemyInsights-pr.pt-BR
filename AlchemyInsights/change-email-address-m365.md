---
title: Alterar endereço de email do grupo do Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416688"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Alterar endereço de email de um grupo do Microsoft 365

Você pode alterar o endereço de email de um grupo do Microsoft 365 no centro de administração. Basta selecionar o grupo e selecionar @edit endereço de e-mail.

Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplo:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
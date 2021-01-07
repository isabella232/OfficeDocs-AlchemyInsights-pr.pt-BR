---
title: Alterar endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756545"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Alterar endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams

Você pode alterar o endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams no [Centro de administração do Microsoft 365](https://admin.microsoft.com/). Basta selecionar o grupo e selecionar @edit endereço de e-mail.

Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplo:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

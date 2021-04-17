---
title: Alterar endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819068"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Alterar endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams

Você pode alterar o endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams no [Centro de administração do Microsoft 365](https://admin.microsoft.com/). Basta selecionar o grupo e selecionar @edit endereço de e-mail.

Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplo:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

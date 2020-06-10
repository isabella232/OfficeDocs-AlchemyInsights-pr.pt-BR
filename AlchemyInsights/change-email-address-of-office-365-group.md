---
title: Alterar endereço de email de um grupo do Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580645"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Alterar endereço de email de um grupo do Microsoft 365

Você pode alterar o endereço de email de um grupo do Microsoft 365 no centro de administração. Basta selecionar o grupo e selecionar @edit endereço de e-mail.

Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exemplo:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

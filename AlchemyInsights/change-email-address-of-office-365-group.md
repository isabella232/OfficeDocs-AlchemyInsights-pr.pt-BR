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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="404d2-102">Alterar endereço de email de um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="404d2-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="404d2-103">Você pode alterar o endereço de email de um grupo do Microsoft 365 no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="404d2-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="404d2-104">Basta selecionar o grupo e selecionar @edit endereço de e-mail.</span><span class="sxs-lookup"><span data-stu-id="404d2-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="404d2-105">Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="404d2-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="404d2-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="404d2-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="404d2-107">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="404d2-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

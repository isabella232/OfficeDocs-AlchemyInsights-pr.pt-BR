---
title: Alterar endereço de e-mail de um grupo do Microsoft 365
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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282173"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="89238-102">Alterar endereço de e-mail de um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="89238-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="89238-103">Você pode alterar o endereço de e-mail de um grupo do Microsoft 365 ao usar o centro de administração.</span><span class="sxs-lookup"><span data-stu-id="89238-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="89238-104">Basta selecionar o grupo e selecionar @edit endereço de e-mail.</span><span class="sxs-lookup"><span data-stu-id="89238-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="89238-105">Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="89238-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="89238-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="89238-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="89238-107">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="89238-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

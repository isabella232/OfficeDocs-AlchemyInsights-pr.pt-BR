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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="3a32f-102">Alterar endereço de email de um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3a32f-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="3a32f-103">Você pode alterar o endereço de email de um grupo do Microsoft 365 no centro de administração.</span><span class="sxs-lookup"><span data-stu-id="3a32f-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="3a32f-104">Basta selecionar o grupo e selecionar @edit endereço de e-mail.</span><span class="sxs-lookup"><span data-stu-id="3a32f-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="3a32f-105">Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="3a32f-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="3a32f-106">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="3a32f-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

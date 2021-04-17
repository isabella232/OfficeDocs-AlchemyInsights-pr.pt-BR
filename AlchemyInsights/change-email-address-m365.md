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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="d7ede-102">Alterar endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d7ede-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="d7ede-103">Você pode alterar o endereço de email de um grupo do Microsoft 365 ou do Microsoft Teams no [Centro de administração do Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="d7ede-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="d7ede-104">Basta selecionar o grupo e selecionar @edit endereço de e-mail.</span><span class="sxs-lookup"><span data-stu-id="d7ede-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="d7ede-105">Você também pode usar o comando EXO PowerShell para alterar o endereço SMTP principal de um grupo do Microsoft 365/Teams:</span><span class="sxs-lookup"><span data-stu-id="d7ede-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="d7ede-106">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="d7ede-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

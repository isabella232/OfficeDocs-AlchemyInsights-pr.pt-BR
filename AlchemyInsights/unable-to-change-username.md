---
title: Não é possível mudar o Nome de Usuário
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798652"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="b12b1-102">Não é possível mudar o Nome de Usuário</span><span class="sxs-lookup"><span data-stu-id="b12b1-102">Unable to change UserName</span></span>

<span data-ttu-id="b12b1-103">Em alguns casos, as alterações de UPN (UserPrincipalName) não são propagadas para a nuvem.</span><span class="sxs-lookup"><span data-stu-id="b12b1-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="b12b1-104">Você pode receber erros de validação no portal do Office 365 ou ser impedido de alterar o nome de usuário ou o endereço de email.</span><span class="sxs-lookup"><span data-stu-id="b12b1-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="b12b1-105">Para resolver esse problema, defina manualmente o UserPrincipalName usando este comando do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b12b1-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="b12b1-106">**Exemplo: Renomear um usuário**</span><span class="sxs-lookup"><span data-stu-id="b12b1-106">**Example: Rename a user**</span></span>

<span data-ttu-id="b12b1-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="b12b1-107">PowerShellCopy</span></span>

<span data-ttu-id="b12b1-108">PS C:\> Set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="b12b1-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="b12b1-109">Esse comando renomeia davidc@contoso.com para davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b12b1-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="b12b1-110">Para mais informações, confira [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="b12b1-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>
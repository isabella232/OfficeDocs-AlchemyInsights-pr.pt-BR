---
title: Não é possível mudar o Nome de Usuário
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431327"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="5b85f-102">Não é possível mudar o Nome de Usuário</span><span class="sxs-lookup"><span data-stu-id="5b85f-102">Unable to change UserName</span></span>

<span data-ttu-id="5b85f-103">Em alguns casos, as alterações de UPN (UserPrincipalName) não são propagadas para a nuvem.</span><span class="sxs-lookup"><span data-stu-id="5b85f-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="5b85f-104">Você pode receber erros de validação no portal do Office 365 ou ser impedido de alterar o nome de usuário ou o endereço de email.</span><span class="sxs-lookup"><span data-stu-id="5b85f-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="5b85f-105">Para resolver esse problema, defina manualmente o UserPrincipalName usando este comando do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5b85f-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="5b85f-106">**Exemplo: Renomear um usuário**</span><span class="sxs-lookup"><span data-stu-id="5b85f-106">**Example: Rename a user**</span></span>

<span data-ttu-id="5b85f-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="5b85f-107">PowerShellCopy</span></span>

<span data-ttu-id="5b85f-108">PS C:\> Set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="5b85f-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="5b85f-109">Esse comando renomeia davidc@contoso.com para davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5b85f-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="5b85f-110">Para mais informações, confira [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="5b85f-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>
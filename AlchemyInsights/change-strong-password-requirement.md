---
title: Alterar um requisito de senha forte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518747"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="12a32-102">Alterar um requisito de senha forte</span><span class="sxs-lookup"><span data-stu-id="12a32-102">Change strong password requirement</span></span>

<span data-ttu-id="12a32-103">A Microsoft requer senhas fortes por padrão.</span><span class="sxs-lookup"><span data-stu-id="12a32-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="12a32-104">Usando o PowerShell, você pode desabilitar senhas fortes para usuários específicos com este comando:</span><span class="sxs-lookup"><span data-stu-id="12a32-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="12a32-105">*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="12a32-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="12a32-106">Mais informações sobre a política de senha</span><span class="sxs-lookup"><span data-stu-id="12a32-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="12a32-107">Como se conectar ao Office 365 com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="12a32-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="12a32-108">Saiba mais sobre os comandos do PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="12a32-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
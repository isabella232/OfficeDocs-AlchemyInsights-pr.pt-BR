---
title: Alterar o requisito de senha forte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070672"
---
# <a name="change-strong-password-requirement"></a>Alterar requisito de senha forte

A Microsoft exige senhas fortes por padrão.

Usando o PowerShell, você pode desabilitar senhas fortes para usuários específicos com estes comandos:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Para desabilitar senhas fortes para todos os usuários, use:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Mais informações sobre a política de senha](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Como se conectar ao Microsoft 365 com o PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Mais informações sobre comandos do PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)

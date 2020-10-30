---
title: Alterar um requisito de senha forte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804411"
---
# <a name="change-strong-password-requirement"></a>Alterar um requisito de senha forte

A Microsoft requer senhas fortes por padrão.

Usando o PowerShell, você pode desabilitar senhas fortes para usuários específicos com estes comandos:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Para desabilitar senhas fortes para todos os usuários, use:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Mais informações sobre a política de senha](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Como se conectar ao Microsoft 365 com o PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Saiba mais sobre os comandos do PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)

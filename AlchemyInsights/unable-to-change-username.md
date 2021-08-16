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
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020216"
---
# <a name="unable-to-change-username"></a>Não é possível mudar o Nome de Usuário

Em alguns casos, as alterações de UPN (UserPrincipalName) não são propagadas para a nuvem. Você pode receber erros de validação no portal do Office 365 ou ser impedido de alterar o nome de usuário ou o endereço de email. Para resolver esse problema, defina manualmente o UserPrincipalName usando este comando do PowerShell.

**Exemplo: Renomear um usuário**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Esse comando renomeia davidc@contoso.com para davidchew@contoso.com.

Para mais informações, confira [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).
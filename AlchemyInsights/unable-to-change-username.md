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
# <a name="unable-to-change-username"></a>Não é possível mudar o Nome de Usuário

Em alguns casos, as alterações de UPN (UserPrincipalName) não são propagadas para a nuvem. Você pode receber erros de validação no portal do Office 365 ou ser impedido de alterar o nome de usuário ou o endereço de email. Para resolver esse problema, defina manualmente o UserPrincipalName usando este comando do PowerShell.

**Exemplo: Renomear um usuário**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Esse comando renomeia davidc@contoso.com para davidchew@contoso.com.

Para mais informações, confira [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).
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
# <a name="unable-to-change-username"></a>Não é possível mudar o Nome de Usuário

Em alguns casos, as alterações de UPN (UserPrincipalName) não são propagadas para a nuvem. Você pode receber erros de validação no portal do Office 365 ou ser impedido de alterar o nome de usuário ou o endereço de email. Para resolver esse problema, defina manualmente o UserPrincipalName usando este comando do PowerShell.

**Exemplo: Renomear um usuário**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName-UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Esse comando renomeia davidc@contoso.com para davidchew@contoso.com.

Para mais informações, confira [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).
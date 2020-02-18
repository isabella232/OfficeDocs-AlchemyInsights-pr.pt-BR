---
title: Conectar-se ao módulo MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093524"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce requer uma conta de administrador de empresa ou cobrança

O módulo MSCommerce requer uma conta com privilégios de administrador da empresa ou de cobrança. Se você estiver recebendo o erro a seguir, será necessário reconectar-se com uma conta diferente.

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

Se sua conta não tiver privilégios de administrador de empresa ou cobrança, entre em contato com seu administrador de ti.

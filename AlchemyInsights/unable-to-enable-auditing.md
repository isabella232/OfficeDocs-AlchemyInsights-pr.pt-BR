---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007778"
---
# <a name="unable-to-enable-unified-auditing"></a>Não é possível habilitar a auditoria unificada

Ao tentar habilitar a auditoria unificada para sua organização, você pode receber um erro semelhante ao seguinte:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Para resolver esse problema, siga estas etapas:

1. [Conexão para Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Execute o seguinte cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Aguarde 60 minutos para que a configuração anterior entre em vigor.

4. Execute o seguinte comando no Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Para obter informações adicionais, consulte os seguintes artigos:

- [Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Ativar ou desativar a pesquisa de log de auditoria](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)

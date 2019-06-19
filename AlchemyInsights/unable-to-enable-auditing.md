---
title: 2419-não é possível habilitar a auditoria
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065597"
---
# <a name="unable-to-enable-unified-auditing"></a>Não é possível habilitar a auditoria unificada

Ao tentar habilitar a auditoria unificada para sua organização do Office 365, você pode receber um erro semelhante ao seguinte:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Para resolver esse problema, siga estas etapas:

1. [Conecte-se ao PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Execute o seguinte cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Aguarde 60 minutos para que a configuração anterior entre em vigor.

4. Execute o seguinte comando no PowerShell do Exchange Online:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Para obter informações adicionais, consulte os seguintes artigos:

- [Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Ativar e desativar a Pesquisa de log de auditoria do Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)

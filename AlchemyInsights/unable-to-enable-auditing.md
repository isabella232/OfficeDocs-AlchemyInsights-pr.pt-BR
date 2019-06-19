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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="8d2fe-102">Não é possível habilitar a auditoria unificada</span><span class="sxs-lookup"><span data-stu-id="8d2fe-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="8d2fe-103">Ao tentar habilitar a auditoria unificada para sua organização do Office 365, você pode receber um erro semelhante ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="8d2fe-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="8d2fe-104">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="8d2fe-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="8d2fe-105">[Conecte-se ao PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="8d2fe-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="8d2fe-106">Execute o seguinte cmdlet:</span><span class="sxs-lookup"><span data-stu-id="8d2fe-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="8d2fe-107">Aguarde 60 minutos para que a configuração anterior entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="8d2fe-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="8d2fe-108">Execute o seguinte comando no PowerShell do Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="8d2fe-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="8d2fe-109">Para obter informações adicionais, consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="8d2fe-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="8d2fe-110">Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator</span><span class="sxs-lookup"><span data-stu-id="8d2fe-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="8d2fe-111">Ativar e desativar a Pesquisa de log de auditoria do Office 365</span><span class="sxs-lookup"><span data-stu-id="8d2fe-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)

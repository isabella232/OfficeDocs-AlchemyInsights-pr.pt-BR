---
title: 2419-não é possível habilitar a auditoria
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510416"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="c528f-102">Não é possível habilitar a auditoria unificada</span><span class="sxs-lookup"><span data-stu-id="c528f-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="c528f-103">Ao tentar habilitar a auditoria unificada para sua organização, você pode receber um erro semelhante ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="c528f-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="c528f-104">Para resolver esse problema, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="c528f-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="c528f-105">[Conecte-se ao PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="c528f-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="c528f-106">Execute o seguinte cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c528f-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="c528f-107">Aguarde 60 minutos para que a configuração anterior entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="c528f-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="c528f-108">Execute o seguinte comando no PowerShell do Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="c528f-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="c528f-109">Para obter informações adicionais, consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="c528f-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="c528f-110">Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator</span><span class="sxs-lookup"><span data-stu-id="c528f-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="c528f-111">Ativar ou desativar a pesquisa de log de auditoria</span><span class="sxs-lookup"><span data-stu-id="c528f-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)

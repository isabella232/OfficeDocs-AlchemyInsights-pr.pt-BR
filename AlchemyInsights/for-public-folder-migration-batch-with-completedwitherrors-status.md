---
title: Para lote de migração de pasta pública com status CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812452"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para lote de migração de pasta pública com status CompletedWithErrors

Use as etapas a seguir para concluir o lote, ignorando os itens grandes/ruins: 
1. Aprovar os itens ignorados em lote de migração:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Use o seguinte comando para aprovar os itens ignorados em solicitações de migração que são "Sincronizadas" mas não concluídas:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. O lote de migração e as solicitações devem ser retomadas e concluídas em alguns minutos.


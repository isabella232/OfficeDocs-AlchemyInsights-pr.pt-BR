---
title: Para lote de migração de pasta pública com status CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158585"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para lote de migração de pasta pública com status CompletedWithErrors

Use as etapas a seguir para concluir o lote, ignorando os itens grandes/ruins: 
1. Aprovar os itens ignorados no lote de migração:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Use o seguinte comando para aprovar os itens ignorados em solicitações de migração que estão "sincronizadas", mas não foram concluídas:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. O lote de migração e as solicitações devem ser retomados e concluídos em alguns minutos.


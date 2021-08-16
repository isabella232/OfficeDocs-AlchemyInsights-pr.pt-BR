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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068152"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para lote de migração de pasta pública com status CompletedWithErrors

Use as etapas a seguir para concluir o lote, ignorando os itens grandes/ruins: 
1. Aprovar os itens ignorados em lote de migração:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Use o seguinte comando para aprovar os itens ignorados em solicitações de migração que são "Sincronizadas" mas não concluídas:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. O lote de migração e as solicitações devem ser retomadas e concluídas em alguns minutos.


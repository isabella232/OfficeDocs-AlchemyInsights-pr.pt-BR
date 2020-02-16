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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043565"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para lote de migração de pasta pública com status CompletedWithErrors

Use as etapas a seguir para concluir o lote, ignorando os itens grandes/ruins: 
1. Aprovar os itens ignorados no lote de migração:

    Set-MigrationBatch \<batchname>-ApproveSkippedItems 
2. Use o seguinte comando para aprovar os itens ignorados em solicitações de migração que estão "sincronizadas", mas não foram concluídas:

    $pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i em $pf) {if ($i. LargeItemsEncountered-gt 0 ou $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:
3. O lote de migração e as solicitações devem ser retomados e concluídos em alguns minutos.


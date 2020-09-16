---
title: Para lote de migração de pasta pública com status CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744101"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="e5ead-102">Para lote de migração de pasta pública com status CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="e5ead-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="e5ead-103">Use as etapas a seguir para concluir o lote, ignorando os itens grandes/ruins:</span><span class="sxs-lookup"><span data-stu-id="e5ead-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="e5ead-104">Aprovar os itens ignorados no lote de migração:</span><span class="sxs-lookup"><span data-stu-id="e5ead-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="e5ead-105">Use o seguinte comando para aprovar os itens ignorados em solicitações de migração que estão "sincronizadas", mas não foram concluídas:</span><span class="sxs-lookup"><span data-stu-id="e5ead-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="e5ead-106">O lote de migração e as solicitações devem ser retomados e concluídos em alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="e5ead-106">The migration batch and requests should resume and complete in a few minutes.</span></span>


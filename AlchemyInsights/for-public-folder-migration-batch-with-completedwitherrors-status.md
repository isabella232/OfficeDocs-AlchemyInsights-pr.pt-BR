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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="28373-102">Para lote de migração de pasta pública com status CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="28373-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="28373-103">Use as etapas a seguir para concluir o lote, ignorando os itens grandes/ruins:</span><span class="sxs-lookup"><span data-stu-id="28373-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="28373-104">Aprovar os itens ignorados no lote de migração:</span><span class="sxs-lookup"><span data-stu-id="28373-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="28373-105">Use o seguinte comando para aprovar os itens ignorados em solicitações de migração que estão "sincronizadas", mas não foram concluídas:</span><span class="sxs-lookup"><span data-stu-id="28373-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="28373-106">O lote de migração e as solicitações devem ser retomados e concluídos em alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="28373-106">The migration batch and requests should resume and complete in a few minutes.</span></span>


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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="ca470-102">Para lote de migração de pasta pública com status CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="ca470-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="ca470-103">Use as etapas a seguir para concluir o lote, ignorando os itens grandes/ruins:</span><span class="sxs-lookup"><span data-stu-id="ca470-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="ca470-104">Aprovar os itens ignorados no lote de migração:</span><span class="sxs-lookup"><span data-stu-id="ca470-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="ca470-105">Set-MigrationBatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="ca470-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="ca470-106">Use o seguinte comando para aprovar os itens ignorados em solicitações de migração que estão "sincronizadas", mas não foram concluídas:</span><span class="sxs-lookup"><span data-stu-id="ca470-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="ca470-107">$pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i em $pf) {if ($i. LargeItemsEncountered-gt 0 ou $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:</span><span class="sxs-lookup"><span data-stu-id="ca470-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="ca470-108">O lote de migração e as solicitações devem ser retomados e concluídos em alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="ca470-108">The migration batch and requests should resume and complete in a few minutes.</span></span>


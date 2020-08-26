---
title: A migração da pasta pública falha em 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903508"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="3818c-102">A migração da pasta pública falha em 95%</span><span class="sxs-lookup"><span data-stu-id="3818c-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="3818c-103">Para migrações de pasta pública falhando em 95%, com o erro FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="3818c-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="3818c-104">Baixar e executar o script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) no servidor local do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3818c-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="3818c-105">Executar as ações corretivas sugeridas pelo script.</span><span class="sxs-lookup"><span data-stu-id="3818c-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="3818c-106">Executar o Sync-MailPublicFolders (para Exchange 2010) ou o Sync-ModernMailPublicFolders (para o Exchange 2013 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="3818c-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="3818c-107">Retomar a migração da pasta pública.</span><span class="sxs-lookup"><span data-stu-id="3818c-107">Resume public folder migration.</span></span>

---
title: A migração da pasta pública falha em 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662418"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="5590d-102">A migração da pasta pública falha em 95%</span><span class="sxs-lookup"><span data-stu-id="5590d-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="5590d-103">Você pode ter iniciado a conclusão de um conjunto de migração, e o status do conjunto de migração continua exibindo **Sincronizado** por um tempo muito longo.</span><span class="sxs-lookup"><span data-stu-id="5590d-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="5590d-104">Esse comportamento é esperado.</span><span class="sxs-lookup"><span data-stu-id="5590d-104">This is expected behavior.</span></span>

<span data-ttu-id="5590d-105">É comum que o status de um conjunto de migração permaneça em **Sincronizado** por algumas horas antes de mudar para **Completar**.</span><span class="sxs-lookup"><span data-stu-id="5590d-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="5590d-106">Para migrações envolvendo um grande número de caixas de correio alvo, é normal ver que o status permaneça no estado de sincronização por mais de 24 horas, desde que nenhum dos pedidos de migração de pastas públicas subjacentes tenha falhado ou tenha sido colocado em quarentena.</span><span class="sxs-lookup"><span data-stu-id="5590d-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="5590d-107">Aguarde de 24 a 48 horas para que o conjunto de migração conclua as tarefas.</span><span class="sxs-lookup"><span data-stu-id="5590d-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="5590d-108">Para migrações de pasta pública falhando em 95%, com o erro FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="5590d-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="5590d-109">Baixar e executar o script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) no servidor local do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5590d-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="5590d-110">Executar as ações corretivas sugeridas pelo script.</span><span class="sxs-lookup"><span data-stu-id="5590d-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="5590d-111">Executar o Sync-MailPublicFolders (para Exchange 2010) ou o Sync-ModernMailPublicFolders (para o Exchange 2013 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="5590d-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="5590d-112">Retomar a migração da pasta pública.</span><span class="sxs-lookup"><span data-stu-id="5590d-112">Resume public folder migration.</span></span>

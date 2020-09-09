---
title: Lote de migração de pasta pública não concluído, mostra sincronizado
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
ms.openlocfilehash: 7a87d8dafae2b0f3ff3f4e1ecdb6e02d73e9caf2
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406530"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="63338-102">Lote de migração de pasta pública não concluído, mostra sincronizado</span><span class="sxs-lookup"><span data-stu-id="63338-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="63338-103">Você pode ter iniciado a conclusão de um lote de migração, e o status do lote de migração continua exibindo Sincronizado por um tempo muito longo.</span><span class="sxs-lookup"><span data-stu-id="63338-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="63338-104">Esse comportamento é esperado.</span><span class="sxs-lookup"><span data-stu-id="63338-104">This is expected behavior.</span></span>

<span data-ttu-id="63338-105">É comum que o status de um lote de migração permaneça em Sincronizado por algumas horas antes de mudar para Completando.</span><span class="sxs-lookup"><span data-stu-id="63338-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="63338-106">Para migrações envolvendo um grande número de caixas de correio alvo, é normal ver que o status permaneça no estado de sincronização por mais de 24 horas, desde que nenhum dos pedidos de migração de pastas públicas subjacentes tenha falhado ou tenha sido colocado em quarentena.</span><span class="sxs-lookup"><span data-stu-id="63338-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="63338-107">Aguarde de 24 a 48 horas para que o lote de migração conclua as tarefas.</span><span class="sxs-lookup"><span data-stu-id="63338-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

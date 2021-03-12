---
title: Conjunto de réplicas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716264"
---
# <a name="replica-set"></a><span data-ttu-id="6cb4b-102">Conjunto de réplicas</span><span class="sxs-lookup"><span data-stu-id="6cb4b-102">Replica set</span></span>

<span data-ttu-id="6cb4b-103">O AADDS também é chamado como o domínio gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="6cb4b-104">Na verdade, são dois controladores de domínio que são executados e mantidos pelo back-end.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="6cb4b-105">Os dois DCs incluem um DC principal e um DC de replicação.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="6cb4b-106">Backups no AADDS (domínio gerenciado) são um processo automatizado gerenciado pela plataforma do Azure.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="6cb4b-107">Em caso de um problema com seu domínio gerenciado, o suporte ao Azure pode ajudá-lo na restauração do backup.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="6cb4b-108">Você cria cada conjunto de réplicas em uma rede virtual.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="6cb4b-109">Cada rede virtual deve ser igualada a todas as outras redes virtuais que hospedam o conjunto de réplicas de um domínio gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="6cb4b-110">Essa configuração cria uma topologia de rede de malha que oferece suporte à replicação de diretório.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="6cb4b-111">Uma rede virtual pode dar suporte a vários conjuntos de réplicas, desde que cada conjunto de réplicas seja em uma sub-rede virtual diferente.</span><span class="sxs-lookup"><span data-stu-id="6cb4b-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="6cb4b-112">Para obter mais detalhes sobre o conjunto de réplicas, consulte [Conjuntos de réplicas de conceitos.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="6cb4b-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>

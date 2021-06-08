---
title: Problemas de desempenho do Microsoft Defender para Ponto de Extremidade no Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783414"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="aec8b-102">Problemas de desempenho do Microsoft Defender para Ponto de Extremidade no Linux</span><span class="sxs-lookup"><span data-stu-id="aec8b-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="aec8b-103">Este artigo serve de guia nas etapas de identificação de problemas de desempenho do Microsoft Defender para Ponto de Extremidade no Linux.</span><span class="sxs-lookup"><span data-stu-id="aec8b-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="aec8b-104">É importante verificar primeiro se o problema que você está enfrentando foi resolvido com a [versão mais recente](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="aec8b-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="aec8b-105">Para iniciar a sua investigação, consulte [Solução de problemas de desempenho do Microsoft Defender para Ponto de Extremidade no Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="aec8b-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="aec8b-106">Exclusões</span><span class="sxs-lookup"><span data-stu-id="aec8b-106">Exclusions</span></span>

<span data-ttu-id="aec8b-107">As exclusões podem ajudar a atenuar os problemas de desempenho.</span><span class="sxs-lookup"><span data-stu-id="aec8b-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="aec8b-108">Analise as suas exclusões antes de começar, para que qualquer risco adicional seja conhecido e documentado.</span><span class="sxs-lookup"><span data-stu-id="aec8b-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="aec8b-109">Para mais informações, confira [Configurar e validar exclusões no Microsoft Defender para Ponto de Extremidade no Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="aec8b-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="aec8b-110">Quando você tem vários arquivos e pastas para excluir e eles estão todos no mesmo ponto de montagem, pode ser mais fácil excluir o ponto de montagem.</span><span class="sxs-lookup"><span data-stu-id="aec8b-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="aec8b-111">A partir da versão 101.22.80 de fevereiro, você pode excluir um ponto de montagem inteiro.</span><span class="sxs-lookup"><span data-stu-id="aec8b-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="aec8b-112">Por exemplo, se /mnt/backup for um ponto de montagem, você pode adicionar /mnt/backup à lista de exclusão executando este comando:</span><span class="sxs-lookup"><span data-stu-id="aec8b-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="aec8b-113">**Observação**: adicionar exclusões aumenta o risco de o malware não ser detectado e deve ser tratado e implementado com cuidado.</span><span class="sxs-lookup"><span data-stu-id="aec8b-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="aec8b-114">Precisa de ajuda?</span><span class="sxs-lookup"><span data-stu-id="aec8b-114">Need Help?</span></span>

<span data-ttu-id="aec8b-115">Para ajudá-lo da maneira mais eficiente, colete os dados de diagnóstico antes de abrir um caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="aec8b-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>

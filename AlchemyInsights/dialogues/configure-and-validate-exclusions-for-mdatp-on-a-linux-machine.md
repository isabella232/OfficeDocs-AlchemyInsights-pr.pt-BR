---
title: Configurar e validar exclusões para MDATP em uma máquina Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568445"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="d6fb9-102">Configurar e validar exclusões para MDATP em uma máquina Linux</span><span class="sxs-lookup"><span data-stu-id="d6fb9-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="d6fb9-103">Você pode excluir determinados arquivos, pastas, processos e arquivos abertos por processo de verificações MDATP.</span><span class="sxs-lookup"><span data-stu-id="d6fb9-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="d6fb9-104">As exclusões ajudam a evitar a detecção incorreta de software e arquivos exclusivos ou personalizados para sua organização.</span><span class="sxs-lookup"><span data-stu-id="d6fb9-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="d6fb9-105">As exclusões também ajudam a reduzir os problemas de desempenho causados pelo MDATP.</span><span class="sxs-lookup"><span data-stu-id="d6fb9-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="d6fb9-106">Para saber mais, consulte [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="d6fb9-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d6fb9-107">As exclusões descritas neste artigo não se aplicam a outros recursos do MDATP para Linux, incluindo a detecção e a resposta do ponto de extremidade (EDR).</span><span class="sxs-lookup"><span data-stu-id="d6fb9-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="d6fb9-108">Os arquivos excluídos usando os métodos descritos neste artigo ainda podem disparar alertas de EDR e outros recursos de detecção.</span><span class="sxs-lookup"><span data-stu-id="d6fb9-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>

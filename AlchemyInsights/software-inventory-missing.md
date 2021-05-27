---
title: O inventário de software está ausente ou impreciso
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658044"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="bf200-102">O inventário de software está ausente ou impreciso</span><span class="sxs-lookup"><span data-stu-id="bf200-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="bf200-103">O inventário de software no TVM (gerenciamento de ameaças e vulnerabilidades) é uma lista de softwares conhecidos da organização com as CPE (Enumerações de Plataforma Comum) oficiais.</span><span class="sxs-lookup"><span data-stu-id="bf200-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="bf200-104">Os produtos de software sem uma CPE oficial não têm vulnerabilidades publicadas.</span><span class="sxs-lookup"><span data-stu-id="bf200-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="bf200-105">O inventário também inclui detalhes, como o nome do fornecedor, o número de fraquezas, as ameaças e o número de dispositivos expostos.</span><span class="sxs-lookup"><span data-stu-id="bf200-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="bf200-106">As alterações de software nos dispositivos geralmente são refletidas em portais de segurança dentro de duas horas.</span><span class="sxs-lookup"><span data-stu-id="bf200-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="bf200-107">No entanto, às vezes isso pode levar mais tempo.</span><span class="sxs-lookup"><span data-stu-id="bf200-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="bf200-108">Atualmente, não há nenhuma maneira de forçar uma sincronização; essa é uma avaliação contínua.</span><span class="sxs-lookup"><span data-stu-id="bf200-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="bf200-109">Se você fez uma alteração de software e a alteração não for refletida com precisão no TVM após 5 horas, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="bf200-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="bf200-110">Verifique a seção de evidências do software para entender como o software foi detectado.</span><span class="sxs-lookup"><span data-stu-id="bf200-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="bf200-111">Certifique-se de que o software tem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf200-111">Make sure that the software is supported.</span></span> <span data-ttu-id="bf200-112">O software pode estar visível apenas no nível do dispositivo, mesmo que atualmente não tenha suporte para o gerenciamento de ameaças e vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="bf200-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="bf200-113">No entanto, apenas dados limitados estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="bf200-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="bf200-114">Para ver as etapas para relatar a imprecisão do portal, confira [Relatar imprecisão](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="bf200-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="bf200-115">**Observação**: relatar uma imprecisão do portal MDE é um canal unidirecional da engenharia.</span><span class="sxs-lookup"><span data-stu-id="bf200-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="bf200-116">Se o problema for urgente, abra um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="bf200-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="bf200-117">Para saber mais, confira [Inventário de software – gerenciamento de ameaças e vulnerabilidades](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="bf200-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>
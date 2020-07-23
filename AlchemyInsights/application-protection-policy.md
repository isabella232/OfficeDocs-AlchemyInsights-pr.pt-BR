---
title: Política de proteção de aplicativos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45266398"
---
# <a name="application-protection-policy"></a><span data-ttu-id="a562d-102">Política de proteção de aplicativos</span><span class="sxs-lookup"><span data-stu-id="a562d-102">Application protection policy</span></span>

<span data-ttu-id="a562d-103">Se você não tiver experiência com as políticas de proteção de aplicativo (APP), confira o [Visão geral das políticas de proteção de aplicativo](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="a562d-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="a562d-104">Para começar a usar o aplicativo, consulte [Como criar e atribuir políticas de proteção de aplicativo](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="a562d-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="a562d-105">Requisitos de política de proteção de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="a562d-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="a562d-106">O usuário tem uma licença do Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="a562d-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="a562d-107">O usuário pertence a um grupo direcionado pelas políticas de proteção de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a562d-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="a562d-108">Somente um usuário corporativo está conectado aos aplicativos protegidos em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a562d-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="a562d-109">O aplicativo implementou o [SDK do Intune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="a562d-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="a562d-110">Para obter uma lista de aplicativos que oferecem suporte ao SDK, confira [Aplicativos protegidos do Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="a562d-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="a562d-111">As políticas se aplicam depois que um usuário que atende aos requisitos acima se inscreve em um aplicativo habilitado para SDK do Intune.</span><span class="sxs-lookup"><span data-stu-id="a562d-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="a562d-112">A maneira mais fácil de determinar se uma política é aplicada é exigindo que o usuário defina um PIN na política.</span><span class="sxs-lookup"><span data-stu-id="a562d-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="a562d-113">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="a562d-113">For more information, see:</span></span>

[<span data-ttu-id="a562d-114">Perguntas frequentes sobre a solução de problemas do APP/MAM</span><span class="sxs-lookup"><span data-stu-id="a562d-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="a562d-115">Como validar a configuração da política de proteção de aplicativos</span><span class="sxs-lookup"><span data-stu-id="a562d-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="a562d-116">Compreender o tempo de entrega da Política de Proteção de Aplicativos</span><span class="sxs-lookup"><span data-stu-id="a562d-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="a562d-117">Como monitorar políticas de proteção de aplicativos</span><span class="sxs-lookup"><span data-stu-id="a562d-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)
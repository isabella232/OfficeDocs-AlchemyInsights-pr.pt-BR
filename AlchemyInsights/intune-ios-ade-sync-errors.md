---
title: Erros de sincronização de registro automático de dispositivo apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448910"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="c1c00-102">Erros de sincronização de registro automático de dispositivo apple</span><span class="sxs-lookup"><span data-stu-id="c1c00-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="c1c00-103">"Detectamos que você tem um ou mais Tokens ADE/DEP que estão em um estado de erro.</span><span class="sxs-lookup"><span data-stu-id="c1c00-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="c1c00-104">Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade do ADE não funcionará conforme esperado.".</span><span class="sxs-lookup"><span data-stu-id="c1c00-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="c1c00-105">Esse erro pode se manifesto de várias maneiras, incluindo:</span><span class="sxs-lookup"><span data-stu-id="c1c00-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="c1c00-106">Os dispositivos podem não sincronizar entre ABM/ASM e Intune</span><span class="sxs-lookup"><span data-stu-id="c1c00-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="c1c00-107">As atribuições de perfil de registro podem estar falhando</span><span class="sxs-lookup"><span data-stu-id="c1c00-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="c1c00-108">Os dispositivos podem não concluir o registro do ADE com êxito</span><span class="sxs-lookup"><span data-stu-id="c1c00-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="c1c00-109">Verifique se o erro de sincronização relatado no console do Intune em **Dispositivos > Registrar Dispositivos >** apple registro > tokens de programa de registro .</span><span class="sxs-lookup"><span data-stu-id="c1c00-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="c1c00-110">Uma das causas mais comuns de erro de sincronização é a expiração do token atual.</span><span class="sxs-lookup"><span data-stu-id="c1c00-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="c1c00-111">Em muitos casos, a renovação do token afetado resolverá o problema.</span><span class="sxs-lookup"><span data-stu-id="c1c00-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="c1c00-112">Se um ou mais de seus tokens expirar, consulte a documentação a seguir para ajudá-lo a renová-los conforme apropriado:</span><span class="sxs-lookup"><span data-stu-id="c1c00-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="c1c00-113">Renovar um token de registro de dispositivo automatizado</span><span class="sxs-lookup"><span data-stu-id="c1c00-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="c1c00-114">Além disso, você pode ver a documentação a seguir para ver possíveis correções de outros erros que causam falhas de sincronização de token:</span><span class="sxs-lookup"><span data-stu-id="c1c00-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="c1c00-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span><span class="sxs-lookup"><span data-stu-id="c1c00-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="c1c00-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span><span class="sxs-lookup"><span data-stu-id="c1c00-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)

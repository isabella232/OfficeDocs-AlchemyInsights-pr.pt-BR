---
title: Erros de sincronização de dispositivos automáticos da Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707852"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="46d3c-102">Erros de sincronização de dispositivos automáticos da Apple</span><span class="sxs-lookup"><span data-stu-id="46d3c-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="46d3c-103">"Detectamos que você tem um ou mais tokens ADE/DEP que estão em um estado de erro.</span><span class="sxs-lookup"><span data-stu-id="46d3c-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="46d3c-104">Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade ADE não funcionará para o mesmo ".</span><span class="sxs-lookup"><span data-stu-id="46d3c-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="46d3c-105">Este erro pode ser manifestado de várias maneiras, incluindo:</span><span class="sxs-lookup"><span data-stu-id="46d3c-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="46d3c-106">Os dispositivos podem não ser sincronizados do ABM/ASM para o Intune</span><span class="sxs-lookup"><span data-stu-id="46d3c-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="46d3c-107">As atribuições de perfil de registro podem estar falhando</span><span class="sxs-lookup"><span data-stu-id="46d3c-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="46d3c-108">Os dispositivos podem não concluir o registro ADE com êxito</span><span class="sxs-lookup"><span data-stu-id="46d3c-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="46d3c-109">Verifique se o erro de sincronização relatado no console do Intune em **dispositivos > inscrever dispositivos > registro da Apple > tokens de programa de registro** e leia a seguinte documentação para ver possíveis remediação:</span><span class="sxs-lookup"><span data-stu-id="46d3c-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="46d3c-110">Erros de sincronização do ABM/ASM para tokens de registro de dispositivo automatizado do iOS/iPadOS e macOS</span><span class="sxs-lookup"><span data-stu-id="46d3c-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)

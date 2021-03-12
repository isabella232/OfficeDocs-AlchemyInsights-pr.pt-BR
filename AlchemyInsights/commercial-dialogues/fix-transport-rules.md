---
title: Corrigir regras de transporte
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735683"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="4090d-102">Corrigir regras de transporte</span><span class="sxs-lookup"><span data-stu-id="4090d-102">Fix transport rules</span></span>

<span data-ttu-id="4090d-103">Uma regra de fluxo de emails personalizada afetou essa mensagem.</span><span class="sxs-lookup"><span data-stu-id="4090d-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="4090d-104">Para revisar a regra exata, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4090d-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="4090d-105">Nos resultados do envio, em **Informações adicionais,** observe **o GUID** ou o Nome **da Política.**</span><span class="sxs-lookup"><span data-stu-id="4090d-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="4090d-106">Iniciar o Shell de Gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4090d-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="4090d-107">Para obter mais informações, [consulte Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="4090d-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="4090d-108">Execute este comando (usando o GUID do envio):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="4090d-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="4090d-109">Revise a descrição para ver as condições configuradas que afetaram a mensagem.</span><span class="sxs-lookup"><span data-stu-id="4090d-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="4090d-110">Para saber mais, confira [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="4090d-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>

---
title: Ativar a tecnologia NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917306"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="c357c-102">Ativar a tecnologia NDI</span><span class="sxs-lookup"><span data-stu-id="c357c-102">Turn on NDI technology</span></span>

<span data-ttu-id="c357c-103">A tecnologia NDI requer duas etapas para ser turned on para um usuário:</span><span class="sxs-lookup"><span data-stu-id="c357c-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="c357c-104">O administrador de locatários deve habilitar a propriedade 'AllowNDIStreaming' em CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="c357c-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="c357c-105">Depois que essa alteração for preenchida, o usuário final deverá ativar a tecnologia NDI® para seu cliente específico a partir de Configurações **> Permissões.**</span><span class="sxs-lookup"><span data-stu-id="c357c-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="c357c-106">Para saber mais, confira [Usar a tecnologia NDI no Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="c357c-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>

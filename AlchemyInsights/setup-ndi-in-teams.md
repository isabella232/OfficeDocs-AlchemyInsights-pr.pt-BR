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
# <a name="turn-on-ndi-technology"></a>Ativar a tecnologia NDI

A tecnologia NDI requer duas etapas para ser turned on para um usuário:

1. O administrador de locatários deve habilitar a propriedade 'AllowNDIStreaming' em CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Depois que essa alteração for preenchida, o usuário final deverá ativar a tecnologia NDI® para seu cliente específico a partir de Configurações **> Permissões.**

Para saber mais, confira [Usar a tecnologia NDI no Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)

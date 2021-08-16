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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023510"
---
# <a name="turn-on-ndi-technology"></a>Ativar a tecnologia NDI

A tecnologia NDI requer duas etapas para serem a a turned on para um usuário:

1. O administrador do locatário deve habilitar a propriedade 'AllowNDIStreaming' em CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Depois que essa alteração for preenchida, o usuário final deverá ativar a tecnologia NDI® para seu cliente específico Configurações > **Permissões**.

Para obter mais informações, [consulte Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).

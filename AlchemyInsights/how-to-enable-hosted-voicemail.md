---
title: Como habilitar a Caixa Postal Hospedada
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318636"
---
# <a name="how-to-enable-hosted-voicemail"></a>Como habilitar a Caixa Postal Hospedada

Para habilitar a Caixa Postal, **HostedVoicemail** deve ser definido como $true.

A **propriedade HostedVoicemail** no usuário usando o PowerShell Remoto (RPS).

Para obter mais informações sobre como se conectar ao RPS, consulte Microsoft Teams Visão geral do [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre como se conectar ao RPS.

1. O Teams administrador deve estar conectado ao PowerShell remoto para Teams.
1. No prompt do PowerShell, o administrador do Teams pode executar **set-csuser user@contoso.com -HostedVoiceMail $true** onde o uri do sip é do usuário em questão.

**Observação**: as alterações nas políticas podem levar até 24 horas para ser replicadas.
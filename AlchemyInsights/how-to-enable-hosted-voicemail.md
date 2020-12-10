---
title: Como habilitar a caixa postal hospedada
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608814"
---
# <a name="how-to-enable-hosted-voicemail"></a>Como habilitar a caixa postal hospedada

Para habilitar a caixa postal, **HostedVoicemail** deve ser definido como $true.

A propriedade **HostedVoicemail** no usuário usando o PowerShell remoto (RPS).

Para obter mais informações sobre como se conectar ao RPS, confira [visão geral do Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre como se conectar ao RPS.

1. O administrador do teams deve estar conectado ao PowerShell remoto para o Teams.
1. No prompt do PowerShell, o administrador do teams pode executar **set-csuser User@contoso.com-HostedVoiceMail $true** onde o URI SIP é do usuário em questão.

> [!NOTE]
> As alterações nas políticas podem levar até 24 horas para serem replicadas.
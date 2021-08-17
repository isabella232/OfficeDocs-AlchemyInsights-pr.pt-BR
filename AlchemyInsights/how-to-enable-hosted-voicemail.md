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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055542"
---
# <a name="how-to-enable-hosted-voicemail"></a>Como habilitar a Caixa Postal Hospedada

Para habilitar a Caixa Postal, **HostedVoicemail** deve ser definido como $true.

A **propriedade HostedVoicemail** no usuário usando o PowerShell Remoto (RPS).

Para obter mais informações sobre como se conectar ao RPS, consulte Microsoft Teams Visão geral do [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre como se conectar ao RPS.

1. O Teams administrador deve estar conectado ao PowerShell remoto para Teams.
1. No prompt do PowerShell, o administrador do Teams pode executar **set-csuser user@contoso.com -HostedVoiceMail $true** onde o uri do sip é do usuário em questão.

> [!NOTE]
> As alterações nas políticas podem levar até 24 horas para ser replicadas.
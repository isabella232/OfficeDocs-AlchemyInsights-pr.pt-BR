---
title: Gravação de chamada 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733837"
---
# <a name="11-call-recording"></a>Gravação de chamada 1:1

Os administradores precisam tomar medidas agora para continuar permitindo que os usuários gravem chamadas 1:1.
 
A partir de 12 de abril de 2021, vamos começar a impor uma nova opção de Política de Chamada do Teams *AllowCloudRecordingForCalls*. 

Atualmente, os recursos de gravação de chamada 1:1 são controlados pela *opção AllowCloudRecording* em Políticas de Reunião do Teams. Se os usuários puderem gravar Reuniões do Teams, eles também poderão gravar chamadas 1:1.

Se você preferir impedir que todos os usuários gravam chamadas 1:1, não é necessário tomar nenhuma ação. A opção de política de *chamada AllowCloudRecordingForCalls* será $False por padrão.

Essa alteração é documentada na seguinte postagem da Central de Mensagens: [(Atualizado) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Política de gravação de chamada Para definir a Opção de Política de Chamada do Teams, você deve usar o [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

Para habilitar o registro de **chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Para desabilitar o registro de chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False


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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314372"
---
# <a name="11-call-recording"></a>Gravação de chamada 1:1

Se o **botão Iniciar Gravação** estiver acinzado em uma chamada 1:1, você precisará alterar as configurações de política do usuário afetado. Para verificar a configuração de política, execute o Diagnóstico do usuário afetado digitando **Diag: Teams 1:1 Gravação de Chamada** acima.     

A partir de 31 de maio de 2021, vamos começar a aplicar uma nova política de chamada Teams *AllowCloudRecordingForCalls*. Antes dessa alteração, a gravação de chamada 1:1 é controlada pela Política de Reunião *AllowCloudRecording* Teams Meeting. Essa alteração é documentada na postagem central de mensagens: [(Atualizado) 1:1 Introdução](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)da política de gravação de chamada.  

*AllowCloudRecordingForCalls*   a opção de política de chamada é definida **como $False** por padrão. Se você preferir impedir que todos os usuários gravam chamadas 1:1, não é necessário tomar nenhuma ação.  

Para habilitar a gravação de chamadas para todos os usuários em chamadas 1:1, use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) para executar o seguinte cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Como alternativa, você pode criar uma nova política e definir  **-AllowCloudRecordingForCalls** para $true e atribuir essa política aos seus usuários. 

Para obter mais informações, consulte 1:1 Controles de Política de [Gravação de Chamada são (Quase!) Aqui](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).

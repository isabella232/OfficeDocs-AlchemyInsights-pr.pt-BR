---
title: Configurações de política de reunião
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825431"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerenciar políticas de reunião no Microsoft Teams

**Observação: pode levar até 24 horas para que as alterações de política entre em vigor para os usuários.** Talvez você não consiga fazer alterações nas políticas recém-criadas imediatamente; aguarde 4 horas e tente modificar uma política recém-criada novamente.

As políticas de reunião são usadas para controlar os recursos que estão disponíveis para os participantes da reunião para reuniões agendadas pelos usuários em sua organização. Alguns recursos das políticas de reunião podem ainda não ser implementados no centro de administração do Teams (eles são rotulados como "em breve" na documentação). Nesse caso, ou se você estiver recebendo um erro como "Não podemos atualizar a política agora, mas tentar novamente mais tarde" no Centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar políticas de reunião do Teams. 

Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:

- Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, consulte Gerenciar políticas de reunião [no Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para fazer alterações de política usando cmdlets do PowerShell, consulte [Visão geral do Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o módulo [do PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) do Skype for Business para políticas de reunião do Teams. 
    - Revise a [documentação dos cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.


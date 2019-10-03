---
title: Configurações de política de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376508"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerenciar políticas de reunião no Microsoft Teams

As políticas de reunião são usadas para controlar os recursos disponíveis para os participantes da reunião para reuniões agendadas por usuários em sua organização. Alguns recursos das políticas de reunião podem não ser implementados no centro de administração do teams ainda (eles estão "em breve" na documentação). Nesse caso, ou se você estiver recebendo um erro como "não é possível atualizar a política agora, mas tentar novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar as políticas de reunião do teams. 

Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:

- Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, confira [gerenciar políticas de reunião no Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Para fazer alterações de política usando cmdlets do PowerShell, consulte [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o [módulo PowerShell do Skype for Business](https://www.microsoft.com/download/details.aspx?id=39366) para as políticas de reunião do teams. 
    - Consulte a [documentação dos cmdlets do *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.

**Observação:** Pode levar até 24 horas para que as alterações de política entrem em vigor para os usuários. Você pode não conseguir fazer alterações em políticas recentemente criadas imediatamente; Aguarde 4 horas e tente modificar novamente uma política recém-criada. Se você ainda tiver problemas, experimente o PowerShell.  
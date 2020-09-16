---
title: Configurações de política de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794322"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerenciar políticas de reunião no Microsoft Teams

**Observação: pode levar até 24 horas para que as alterações de política entrem em vigor para os usuários.** Você pode não conseguir fazer alterações em políticas recentemente criadas imediatamente; Aguarde 4 horas e tente modificar novamente uma política recém-criada.

As políticas de reunião são usadas para controlar os recursos disponíveis para os participantes da reunião para reuniões agendadas por usuários em sua organização. Alguns recursos das políticas de reunião podem não ser implementados no centro de administração do teams ainda (eles estão "em breve" na documentação). Nesse caso, ou se você estiver recebendo um erro como "não é possível atualizar a política agora, mas tentar novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar as políticas de reunião do teams. 

Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:

- Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, confira [gerenciar políticas de reunião no Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para fazer alterações de política usando cmdlets do PowerShell, consulte [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o [módulo PowerShell do Skype for Business](https://www.microsoft.com/download/details.aspx?id=39366) para as políticas de reunião do teams. 
    - Consulte a [documentação dos cmdlets do *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.


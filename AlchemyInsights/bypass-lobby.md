---
title: Bypass lobby
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820022"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlar configurações de lobby e nível de participação no Teams

Se você quiser permitir que todos, incluindo usuários dial-in, externos e anônimos, ignorem o **lobby,** use o PowerShell para realizar essa tarefa. Aqui está um exemplo de modificação da política de reunião global para sua organização.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Atualmente, esse cmdlet requer o uso do módulo Do PowerShell do Skype for Business. Para configurar para usar esse cmdlet, confira [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Depois de configurar uma política, você precisa aplicá-la aos usuários; ou, se você modificou a política Global, ela será automaticamente aplicada aos usuários. Para qualquer alteração de política, você precisa aguardar pelo menos 4 horas até **24** horas para que as políticas entre em vigor. 

Não deixe de revisar a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Noções básicas sobre controles de política de lobby de reunião do Teams

Essas configurações controlam quais participantes da reunião aguardam no lobby antes de ser admitidos na reunião e o nível de participação que eles são permitidos em uma reunião. Você pode usar o PowerShell para atualizar as configurações de política de reunião que ainda não foram implementadas (rotuladas como "em breve") no centro de administração do Teams. Confira abaixo um exemplo de cmdlet do PowerShell que permite que todos os usuários ignorem o lobby.

- [Admitir automaticamente que](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) as pessoas são uma política por organizador que controla se as pessoas ingressarão em uma reunião diretamente ou aguardarão no lobby até que sejam admitidas por um usuário autenticado.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Permitir que pessoas anônimas iniciem uma reunião é uma política por organizador que controla se pessoas anônimas, incluindo usuários B2B e federados, podem ingressar na reunião do usuário sem um usuário autenticado da organização presente.

- Permitir que os usuários de discagem ignorem o lobby **(** em breve ) é uma política por organizador que  controla se as pessoas que discam por telefone in unem a reunião diretamente ou aguardam no [lobby,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) independentemente da configuração Admitir automaticamente as pessoas.

- Permitir que os organizadores substituam as configurações de [lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(** em breve ) é uma política  por organizador que controla se o organizador da reunião pode substituir as configurações de lobby definidas por um administrador em Automaticamente admitir pessoas e permitir que os usuários de discagem ignorem o **lobby** quando agendam uma nova reunião.

**Observação:** Leia [Gerenciar políticas de reunião no Teams para](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) uma visão geral completa das políticas de reunião do Microsoft Teams.

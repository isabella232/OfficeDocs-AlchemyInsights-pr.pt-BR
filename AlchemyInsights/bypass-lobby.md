---
title: Ignorar lobby
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684938"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlar as configurações de lobby e o nível de participação no Microsoft Teams

Se quiser permitir que todos, incluindo usuários de discagem, externos e anônimos, **ignore o lobby**, use o PowerShell para realizar essa tarefa. Veja um exemplo de modificação da política de reunião global para sua organização.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Atualmente, este cmdlet requer o uso do módulo PowerShell do Skype for Business. Para ser configurado para usar este cmdlet, confira o [Gerenciamento de políticas por meio do PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Depois de configurar uma política, você precisa aplicá-la aos usuários; ou, se você modificou a política global, ela será automaticamente aplicada aos usuários. Para qualquer alteração de política, você precisa aguardar pelo menos **4 horas até 24 horas** para que as políticas entrem em vigor. 

Leia a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Noções básicas sobre controles de política de lobby de reunião de equipe

Essas configurações controlam quais participantes da reunião esperam no lobby antes de serem admitidos na reunião e o nível de participação que eles são permitidos em uma reunião. Você pode usar o PowerShell para atualizar as configurações de política de reunião que ainda não foram implementadas (rotuladas "em breve") no centro de administração do teams. Veja a seguir um exemplo de cmdlet do PowerShell que permite que todos os usuários ignorem o lobby.

- [Admitir pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas ingressam em uma reunião diretamente ou esperam no lobby até que sejam admitidas por um usuário autenticado.

- [Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo usuários B2B e federados, podem participar da reunião do usuário sem um usuário autenticado da organização em atendimento.

- [Permitir que os usuários discados ignorem o lobby (em](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **breve**) é uma política por organizador que controla se as pessoas que discam por telefone ingressam na reunião diretamente ou esperam no lobby independentemente da configuração **admitir pessoas automaticamente** .

- [Permitir que os organizadores substituam as configurações de lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (em**breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações de lobby de que um administrador definido **automaticamente admite pessoas** e **permitir que os usuários de discagem ignorem o lobby** quando agendarem uma nova reunião.

**Observação:** Leia [gerenciar políticas de reunião no Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das políticas de reunião do Microsoft Teams.

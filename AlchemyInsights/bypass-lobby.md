---
title: Ignorar lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654244"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Controlar configurações de lobby e nível de participação

Se quiser permitir que todos, incluindo usuários de discagem, externos e anônimos para ignorar o lobby, você pode usar o PowerShell para fazer isso. Veja um exemplo de como modificar a política de reunião global para sua organização:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Atualmente, este cmdlet requer o uso do módulo PowerShell do Skype for Business. Para fazer com que a instalação Use este cmdlet, confira [Gerenciamento de políticas por meio do PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Você pode configurar uma nova política, que deverá ser aplicada aos usuários. Se você modificar a política global, ela será automaticamente aplicada aos usuários. Para qualquer alteração de política, você precisa aguardar pelo menos 4 horas e até 24 horas para que as políticas entrem em vigor.

Leia a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Noções básicas sobre controles de política de lobby de reunião de equipe

- [Admitir pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas ingressam em uma reunião diretamente ou esperam no lobby até que sejam admitidas por um usuário autenticado.

- [Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo usuários B2B e federados, podem participar da reunião do usuário sem um usuário autenticado da organização em atendimento.

- [Permitir que os usuários discados ignorem o lobby (em](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **breve**) é uma política por organizador que controla se as pessoas que discam por telefone ingressam na reunião diretamente ou esperam no lobby independentemente da configuração **admitir pessoas automaticamente** .

- [Permitir que os organizadores substituam as configurações de lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (em**breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações de lobby de que um administrador definido em **admitir pessoas** e **permitir discagem os usuários ignoram o lobby** quando eles agendam uma nova reunião.

**Observação:** Leia [gerenciar políticas de reunião no Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das políticas de reunião do Microsoft Teams.

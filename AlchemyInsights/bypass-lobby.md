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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376513"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Controlar configurações de lobby e nível de participação

Essas configurações controlam quais participantes da reunião esperam no lobby antes de serem admitidos na reunião e o nível de participação que eles são permitidos em uma reunião. Você pode usar o PowerShell para atualizar as configurações de política de reunião que ainda não foram implementadas (rotuladas "em breve") no centro de administração do teams.  Veja a seguir um exemplo de cmdlet do PowerShell que permite que todos os usuários ignorem o lobby.  

- [Admitir pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas ingressam em uma reunião diretamente ou esperam no lobby até que sejam admitidas por um usuário autenticado.

- [Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo usuários B2B e federados, podem participar da reunião do usuário sem um usuário autenticado da organização em atendimento.

- [Permitir que os usuários discados ignorem o lobby (em](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **breve**) é uma política por organizador que controla se as pessoas que discam por telefone ingressam na reunião diretamente ou esperam no lobby independentemente da configuração **admitir pessoas automaticamente** .

- [Permitir que os organizadores substituam as configurações de lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (em**breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações de lobby de que um administrador definido em **admitir pessoas** e **permitir discagem os usuários ignoram o lobby** quando eles agendam uma nova reunião.

**Observação:** Leia [gerenciar políticas de reunião no Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das políticas de reunião do Microsoft Teams. 


**Exemplo do PowerShell**

Se quiser permitir que todos, incluindo usuários externos ou anônimos, ignore o lobby, você também pode usar o PowerShell para realizar essa tarefa.  Veja um exemplo de modificação da política de reunião global para sua organização.   

(Verifique a documentação acima antes de fazer essas alterações para entender exatamente o que isso permite).

Set-CsTeamsMeetingPolicy-Identity global-AutoAdmittedUsers "Everyone"-AllowPSTNUsersToBypassLobby $True

Para obter mais informações, consulte [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).

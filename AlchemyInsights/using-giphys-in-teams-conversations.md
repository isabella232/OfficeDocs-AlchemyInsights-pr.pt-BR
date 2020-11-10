---
title: Usando o Giphys em conversas do teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947474"
---
# <a name="using-giphys-in-teams-conversations"></a>Usando o Giphys em conversas do teams

O acesso Giphys no Microsoft Teams está habilitado por padrão. Como administrador, você pode controlar se o Giphys está disponível para os usuários [Configurando uma política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) e garantindo que o **uso do Giphys em conversas** esteja **ativado**.

Se GIFs não estiverem funcionando conforme o esperado nas conversas de equipes, verifique:

A [política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) precisa permitir o Giphys. Para verificar usando os cmdlets do PowerShell:

- Verifique se você pode [gerenciar o Microsoft Teams com o PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Execute o comando do PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verifique se **AllowGiphy** está definido como **true**.
- Se **AllowGiphy** estiver definido como **false** , execute o seguinte comando [set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)do PowerShell.

[Experiências conectadas opcionais](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) precisam ser habilitadas para permitir o acesso à URL do Giphy.

> [!NOTE]
> Se você tiver várias políticas de mensagens do Microsoft Teams configuradas para seu locatário, é possível determinar a identidade da política atribuída ao usuário afetado com o comando [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | do PowerShell. <user@domain.com> Selecione TeamsMessagingPolicy.

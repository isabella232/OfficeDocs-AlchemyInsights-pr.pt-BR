---
title: Usando Giphys em Teams Conversas
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323508"
---
# <a name="using-giphys-in-teams-conversations"></a>Usando Giphys em Teams Conversas

O acesso giphys Teams chat está habilitado por padrão. Como administrador, você pode controlar se Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) está disponível para os usuários definindo uma política de mensagens e garantindo que **Use Giphys** em conversas está **on**.

Se os GIFs não estão funcionando conforme o esperado em Teams conversas, verifique:

A [política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) precisa permitir Giphys. Para verificar usando cmdlets do PowerShell:

- Verifique se você pode [Gerenciar Teams com o PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Execute o comando [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verifique se **AllowGiphy** está definido como **TRUE**.
- Se **AllowGiphy** estiver definido como **FALSE**, execute o seguinte comando do PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Experiências Conectadas Opcionais](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) precisam ser habilitadas para permitir o acesso à URL Giphy.

**Observação**: se você tiver várias políticas de Mensagens Teams configuradas para seu locatário, poderá determinar a identidade da política atribuída ao usuário afetado com o comando [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selecione TeamsMessagingPolicy.

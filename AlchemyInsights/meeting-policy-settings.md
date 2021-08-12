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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925153"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerenciar políticas de reunião em Microsoft Teams

**Observação: pode levar até 24 horas para que as alterações de política entre em vigor para os usuários.** Talvez você não consiga fazer alterações nas políticas recém-criadas imediatamente; aguarde 4 horas e tente modificar uma política recém-criada novamente.

As políticas de reunião são usadas para controlar os recursos disponibilizados para os participantes de reuniões programadas pelos usuários de sua organização. Alguns recursos das políticas de reunião podem não ser implementados no centro de administração Teams ainda (eles são rotulados como "em breve" na documentação). Nesse caso, ou se você estiver recebendo um erro como "Não podemos atualizar a política agora, mas tentar novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar Teams políticas de reunião. 

Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:

- Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, consulte [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para fazer alterações de política usando cmdlets do PowerShell, [consulte Teams Visão Geral do PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o módulo [Skype for Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) para Teams de reunião. 
    - Revise a [documentação dos cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.


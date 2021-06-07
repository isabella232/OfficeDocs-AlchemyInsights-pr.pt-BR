---
title: Gerenciar o registro de webinars
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783136"
---
# <a name="manage-webinar-registration"></a>Gerenciar o registro de webinars

Você gerencia quem pode se registrar nos Webinars do Teams usando os comandos do Powershell do Teams. Para instalar o Powershell do Teams, consulte [PowerShell do Teams](/microsoftteams/teams-powershell-install). 

Por padrão, *WhoCanRegister* está habilitado e definido para **EveryoneInCompany**. Para permitir que qualquer pessoa, incluindo usuários anônimos, se registrem, você deve definir a Política de Reunião para **Todos** usando o Comando do Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Observação**: Se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars. Para saber mais e habilitar essa configuração, consulte [Gerenciar configurações de reunião no Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.

Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).

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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798632"
---
# <a name="manage-webinar-registration"></a>Gerenciar o registro de webinars

Você gerencia quem pode se registrar nos Webinars do Teams usando os comandos do Powershell do Teams. Para instalar o Powershell do Teams, consulte [PowerShell do Teams](/microsoftteams/teams-powershell-install). 

Por padrão, *WhoCanRegister* está habilitado e definido como **Todos**. 

Se você não vir a opção de permitir o registro de Todos no convite da reunião, execute novamente a configuração de *WhoCanRegister* como Todos e aguarde 24 horas. Para executar novamente *WhoCanRegister*, use o comando Windows Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Observação**: Se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars. Para saber mais e habilitar essa configuração, consulte [Gerenciar configurações de reunião no Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.

Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).

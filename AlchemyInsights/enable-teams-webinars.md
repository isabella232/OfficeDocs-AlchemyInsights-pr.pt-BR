---
title: Habilitar os Webinars do Microsoft Teams
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760819"
---
# <a name="enable-teams-webinars"></a>Habilitar os Webinars do Microsoft Teams

Webinars estão habilitados por padrão. Você pode gerenciar quem pode agendar e se registrar para os Webinars do Microsoft Teams usando os comandos do PowerShell do Microsoft Teams.

- Todos os usuários que podem criar uma reunião também podem criar uma reunião webinar. Se você quer gerenciar quem pode agendar os Webinars do Teams, use *AllowMeetingRegistration*. 
- Por padrão, *WhoCanRegister* está habilitado e definido para **Todos**. Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.

Para alterar essas configurações, você deve instalar o [PowerShell do Microsoft Teams](/microsoftteams/teams-powershell-install). Além disso, as Políticas de Reunião são aplicadas nos Webinars do Microsoft Teams. Por exemplo, se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars.

Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).
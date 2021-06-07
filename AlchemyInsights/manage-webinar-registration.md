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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760817"
---
# <a name="manage-webinar-registration"></a>Gerenciar o registro de webinars

Você pode gerenciar quem pode se registrar nos Webinars do Microsoft Teams usando os comandos do PowerShell do Microsoft Teams. Por padrão, *WhoCanRegister* está habilitado e definido para **Todos**. Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.

Para alterar essas configurações, você deve instalar o [PowerShell do Microsoft Teams](/microsoftteams/teams-powershell-install). Além disso, as Políticas de Reunião são aplicadas nos Webinars do Microsoft Teams. Por exemplo, se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars.

Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).
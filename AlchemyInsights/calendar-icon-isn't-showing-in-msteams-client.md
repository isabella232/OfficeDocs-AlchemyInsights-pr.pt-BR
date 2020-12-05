---
title: O ícone de calendário não aparece no cliente do Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576348"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>O ícone de calendário não aparece no cliente do Microsoft Teams

A guia **calendário** no Teams requer acesso a uma caixa de correio do Exchange por meio dos serviços Web do Exchange. A caixa de correio do Exchange pode estar online ou no local. Para usuários online que não vêem a guia **calendário** , verifique se eles [estão licenciados para uma caixa de correio do Exchange Online e se a caixa de correio está habilitada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Se os seus usuários estiverem hospedados no local, você precisará confirmar se sua configuração híbrida está íntegra. Use o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar problemas. Observe que [o Teams exige o Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Para obter mais informações e etapas de solução de problemas, confira [solucionar problemas de interação do Microsoft Teams e do Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).

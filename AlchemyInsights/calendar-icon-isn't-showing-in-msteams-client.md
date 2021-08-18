---
title: Ícone de calendário não está sendo exibido no Microsoft Teams cliente
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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54119992"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ícone de calendário não está sendo exibido no Microsoft Teams cliente

A **Guia** Calendário no Teams requer acesso a uma caixa de correio Exchange por meio Exchange Web Services. A Exchange caixa de correio pode ser Online ou Local. Para usuários online que  não veem a Guia Calendário, certifique-se de que eles estão licenciados para uma caixa de correio Exchange Online e a caixa de correio [está habilitada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Se seus usuários estão no local, você precisa confirmar se sua configuração híbrida está íntegre. Use o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar problemas. Observe que [o Teams exige o Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Para obter mais informações e etapas de solução de problemas, consulte [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).

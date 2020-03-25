---
title: Ícone de calendário não exibido no cliente do Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931816"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ícone de calendário não exibido no cliente do Teams

A guia Calendário no Teams exige acesso a uma caixa de correio do Exchange através dos Serviços Web do Exchange. A caixa de correio do Exchange pode ser Online ou Local. Para os usuários Online que não veem a guia Calendário, certifique-se de que eles [estejam licenciados para uma caixa de correio do Exchange Online e que a caixa de correio esteja habilitada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Se o usuário tem uma caixa de correio válida no Exchange Online, mas ainda não consegue ver a guia Calendário, você pode estar enfrentando um problema de rede. Use o [Analisador de Conectividade Remota da Microsoft](https://testconnectivity.microsoft.com/) e execute os **Testes de Conectividade dos Serviços Web do Microsoft Exchange** para o usuário afetado.

Por fim, confira as [Políticas de configuração de aplicativos – aplicativos do Teams](https://admin.teams.microsoft.com/policies/app-setup) para garantir que o aplicativo de Calendário não tenha sido removido da política aplicada ao usuário (provavelmente a **Global (padrão de toda a organização)**.

Se os usuários estiverem hospedados No Local, você precisa confirmar se a configuração híbrida está íntegra. Use o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar problemas.

Observe que [o Teams exige o Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

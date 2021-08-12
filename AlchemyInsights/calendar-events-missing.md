---
title: Eventos de calendário ausentes ou desatualizados
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: af45345bc8779489f5e00dcaee136103e674068e29c77d8c536d012f475c33c5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968664"
---
# <a name="calendar-events-missing-or-not-updating"></a>Eventos de Calendário ausentes ou desatualizados

Se os itens do calendário estiverem ausentes ou desatualizados, comece por analisando a contagem dos itens nas propriedades da pasta Calendário no Outlook: 

1. Clique com o botão direito do mouse na pasta **Calendário** do usuário afetado e, em seguida, selecione **Propriedades**.

1. Selecione a guia **Sincronização**.

Se a contagem de itens não for a mesma entre a Pasta do Servidor e a Pasta Offline:

1.  Realce a pasta **Calendário**.

1.  Vá para a guia **Enviar**/**Receber** e selecione **Atualizar Pasta**.

Se o calendário ainda estiver desatualizado, ou se os eventos estiverem ausentes, baixe a Ferramenta de Verificação de Calendário para Outlook no [Centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=28786). Determine se há mais de 5.000 itens na pasta do calendário, pois isso poderá causar sintomas como reuniões de calendário desatualizadas ou erros de reunião. 

Para saber mais, confira [Problemas de desempenho do Outlook quando há vários itens ou pastas em um arquivo .ost ou .pst em modo cache](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).
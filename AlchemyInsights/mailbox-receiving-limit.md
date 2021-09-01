---
title: Imposição de limite de recebimento de caixa de correio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829142"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Imposição de limite de recebimento de caixa de correio

Recentemente, a Microsoft começou a impor o limite de 3.600 mensagens por hora por caixa de correio. Para obter mais informações, confira [Limites do Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). As caixas de correio do Microsoft 365 que recebem mais de 3.600 mensagens dentro de uma hora estão limitadas pelos próximos 60 minutos. 

Além disso, o limite de pares de remetente-destinatário (SRP) que bloqueia mensagens recebidas por uma caixa de correio do Microsoft 365 de um remetente específico é aplicado. Se um único remetente enviar mais de 33% do limite total ou 1.200 mensagens por hora sem interrupção para um destinatário específico, o limite de SRP será ativado e a caixa de correio não aceitará mais mensagens desse remetente. Observe que:

- Esse limite é o aplicativo para emails recebidos de outros locatários, locais ou remetentes da Internet.
- A entrega de email para a caixa de correio está bloqueada pelos próximos 60 minutos. 
- Os remetentes dessas caixas de correio recebem um relatório de não entrega (5.2.121 ou 5.2.122) informando que a caixa de correio excedeu o limite máximo de entrega. O intralocatário (email dentro do mesmo locatário) continua a ser entregue.
- Quando o limite de SRP é aplicado, a caixa de correio destinatária continua aceitando mensagens de outros remetentes.

Os administradores podem monitorar a atividade atual da caixa de correio acessando um novo relatório e insight no Centro de administração do Exchange chamado "Caixas de correio que excedem os limites de recebimento". O insight só será exibido se um locatário tiver caixas de correio ofensivos, enquanto o relatório sempre aparece no painel, mas está vazio, a menos que um locatário tenha caixas de correio ofensivos.

Para obter mais informações sobre o insight de limites de recebimento, consulte [Caixas de correio que excedem o insight de limites de recebimento no novo EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Para obter mais informações sobre o relatório de limites de recebimento excedidos, consulte [Relatório de caixas de correio que excedem os limites de recebimento no novo EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).
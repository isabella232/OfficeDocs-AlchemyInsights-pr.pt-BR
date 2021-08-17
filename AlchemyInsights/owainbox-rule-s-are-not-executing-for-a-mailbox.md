---
title: 1332 OWA - As regras de caixa de entrada não estão sendo executadas para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040890"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Uma regra de Caixa de Entrada não funciona conforme o esperado

Verifique as seguintes configurações em Outlook na Web:

- Uma mensagem pode ser redirecionada, encaminhada ou respondeda automaticamente com base em regras de Caixa de Entrada apenas uma vez. Uma regra de redirecionamento (uma regra de caixa de entrada ou regra de fluxo de emails, também conhecida como regra de transporte) pode adicionar no máximo dez destinatários de encaminhamento a uma mensagem. Para obter mais informações, consulte [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- As regras de caixa de entrada não funcionam na caixa de correio de diário alternativa. Para obter mais informações sobre a caixa de correio de diário alternativa, consulte [Caixa de correio de diário alternativo.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Para corrigir esses problemas, consulte [KB 2829319](https://support.microsoft.com/kb/2829319).

Se os problemas anteriores não se aplicarem, execute o relatório de diagnóstico de regra de Caixa de Entrada antes de escalonar o problema para o Suporte da Microsoft:

1. Abra a caixa de correio Outlook na Web e clique em <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Configurações**  >  **Exibir todos os Outlook Configurações**  >  **Email**  >  **Regras**.

2. Na parte inferior da página, clique em **Se suas regras não estão funcionando, clique aqui para gerar um relatório de diagnóstico.**

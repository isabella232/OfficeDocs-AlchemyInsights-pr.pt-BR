---
title: Precisa de ajuda com os limites de envio de e-mails?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702351"
---
# <a name="need-help-with-email-sending-limits"></a>Precisa de ajuda com os limites de envio de e-mails?

Veja a seguir o **limite de envio por design** impostos no serviço. Para saber mais sobre esses limites, confira [aqui](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- Para desencorajar a entrega de mensagens não solicitadas em massa, aplicamos **limites de taxa de destinatário por usuário a todas as mensagens de saída e internas**. Em todas as SKUs, esse limite é de **10.000 destinatários por dia**.  Os clientes que precisam enviar emails comerciais legítimos em massa (por exemplo, boletins informativos para clientes) devem usar provedores de terceiros especializados nesses serviços.
    - **Observação**: Após o limite ter sido atingido, não será mais possível enviar mensagens da caixa de correio até que o número de destinatários para os quais foram enviadas mensagens nas últimas 24 horas fique abaixo do limite. O usuário não poderá enviar mensagens até esse ponto.
- A taxa limite de mensagem de **30 mensagens por minuto** são aplicadas a todas as SKUs. Isso determina quantas mensagens um usuário pode enviar de suas contas do Exchange Online dentro de um período especificado.
- O **número máximo de destinatários permitidos nos campos Para, CC e CCO** para uma única mensagem de email, em todas as SKUs, é **1000 destinatários**. Para personalizar esse limite, veja [aqui](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).

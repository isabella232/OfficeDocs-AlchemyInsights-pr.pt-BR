---
title: Email de saída para a pasta lixo eletrônico
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
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769171"
---
# <a name="outbound-email-to-junk-email-folder"></a>Email de saída para a pasta lixo eletrônico

Se você estiver vendo mensagens de saída marcadas como lixo eletrônico, siga estas etapas:

- Se você ainda não tiver feito isso, considere [configurar notificações de política de spam de saída](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).

- Use o [rastreamento de mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) para ver se a mensagem de saída tem o valor do evento **spam** com detalhes adicionais: **usar pool de entrega de alto risco**.

  Para essas mensagens, verifique o conteúdo da mensagem para ver o que pode ser considerado spam. Por exemplo, as assinaturas podem, às vezes, causar problemas para muitos usuários.

  Se você tiver vários exemplos de mensagens de saída legítimas que estão sendo marcadas como lixo eletrônico, abra um tíquete de suporte e peça ao agente de suporte para enviar suas mensagens como falso positivos para nossos analistas de spam. Esteja preparado para fornecer amostras de mensagens que incluam todos os cabeçalhos de mensagens.

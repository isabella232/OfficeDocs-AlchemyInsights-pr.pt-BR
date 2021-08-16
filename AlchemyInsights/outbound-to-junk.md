---
title: Email de saída para pasta Lixo Eletrônico
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
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096646"
---
# <a name="outbound-email-to-junk-email-folder"></a>Email de saída para pasta Lixo Eletrônico

Se você estiver vendo mensagens de saída sendo marcadas como Lixo Eletrônico, faça as seguintes etapas:

- Se você ainda não tiver feito isso, considere [configurar notificações de](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)política de spam de saída.

- Use [o rastreamento de](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) mensagem para ver se a mensagem de saída tem o valor de evento **Spam** com o detalhe adicional: Use pool de entrega de **alto risco.**

  Para essas mensagens, verifique o conteúdo da mensagem para ver o que pode ser considerado spam. Por exemplo, assinaturas podem causar problemas para muitos usuários.

  Se você tiver vários exemplos de mensagens de saída legítimas que estão sendo marcadas como Lixo Eletrônico, abra um tíquete de suporte e peça ao agente de suporte para enviar suas mensagens como falsos positivos para nossos analistas de spam. Prepare-se para fornecer mensagens de exemplo que incluem todos os headers de mensagens.

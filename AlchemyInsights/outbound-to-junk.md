---
title: Email de saída para a pasta lixo eletrônico
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761156"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="7fe0b-102">Email de saída para a pasta lixo eletrônico</span><span class="sxs-lookup"><span data-stu-id="7fe0b-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="7fe0b-103">Se você estiver vendo mensagens de saída marcadas como lixo eletrônico, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="7fe0b-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="7fe0b-104">Se você ainda não tiver feito isso, considere [configurar notificações de política de spam de saída](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="7fe0b-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="7fe0b-105">Use o [rastreamento de mensagens](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) para ver se a mensagem de saída tem o valor do evento **spam** com detalhes adicionais: **usar pool de entrega de alto risco**.</span><span class="sxs-lookup"><span data-stu-id="7fe0b-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="7fe0b-106">Para essas mensagens, verifique o conteúdo da mensagem para ver o que pode ser considerado spam.</span><span class="sxs-lookup"><span data-stu-id="7fe0b-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="7fe0b-107">Por exemplo, as assinaturas podem, às vezes, causar problemas para muitos usuários.</span><span class="sxs-lookup"><span data-stu-id="7fe0b-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="7fe0b-108">Se você tiver vários exemplos de mensagens de saída legítimas que estão sendo marcadas como lixo eletrônico, abra um tíquete de suporte e peça ao agente de suporte para enviar suas mensagens como falso positivos para nossos analistas de spam.</span><span class="sxs-lookup"><span data-stu-id="7fe0b-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="7fe0b-109">Esteja preparado para fornecer amostras de mensagens que incluam todos os cabeçalhos de mensagens.</span><span class="sxs-lookup"><span data-stu-id="7fe0b-109">Be prepared to provide sample messages that include all message headers.</span></span>

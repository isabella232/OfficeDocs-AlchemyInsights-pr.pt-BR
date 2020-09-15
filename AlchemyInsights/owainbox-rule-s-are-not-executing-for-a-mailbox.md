---
title: 1332 OWA-regra (s) de caixa de entrada não estão sendo executadas para uma caixa de correio
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
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721579"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="aae77-102">Uma regra de caixa de entrada não funciona como esperado</span><span class="sxs-lookup"><span data-stu-id="aae77-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="aae77-103">Verifique as seguintes configurações no Outlook na Web:</span><span class="sxs-lookup"><span data-stu-id="aae77-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="aae77-104">Uma mensagem pode ser redirecionada, encaminhada ou respondida automaticamente com base nas regras de caixa de entrada apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="aae77-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="aae77-105">Uma regra de redirecionamento (uma regra de caixa de entrada ou regra de fluxo de emails, também conhecida como regra de transporte) pode adicionar no máximo dez destinatários de encaminhamento a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="aae77-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="aae77-106">Para saber mais, confira [limites de regras de diário, transporte e caixa de entrada](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="aae77-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="aae77-107">As regras de caixa de entrada não funcionam na caixa de correio de registro em diário alternativa.</span><span class="sxs-lookup"><span data-stu-id="aae77-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="aae77-108">Para obter mais informações sobre a caixa de correio de registro no diário alternativo, confira [caixa de correio de registro em diário alternativo](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="aae77-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="aae77-109">Para corrigir esses problemas, confira [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="aae77-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="aae77-110">Se os problemas anteriores não se aplicarem, execute o relatório de diagnóstico da regra de caixa de entrada antes de escalonar o problema para o suporte da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="aae77-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="aae77-111">Abra a caixa de correio no Outlook na Web e clique em</span><span class="sxs-lookup"><span data-stu-id="aae77-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="aae77-112">**Configurações**  >  do **Exibir todas as configurações**  >  do Outlook **Email**  >  **Regras**.</span><span class="sxs-lookup"><span data-stu-id="aae77-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="aae77-113">Na parte inferior da página, clique em **se suas regras não estiverem funcionando, clique aqui para gerar um relatório de diagnóstico**.</span><span class="sxs-lookup"><span data-stu-id="aae77-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>

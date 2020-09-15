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
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="b6801-102">Precisa de ajuda com os limites de envio de e-mails?</span><span class="sxs-lookup"><span data-stu-id="b6801-102">Need help with email sending limits?</span></span>

<span data-ttu-id="b6801-103">Veja a seguir o **limite de envio por design** impostos no serviço.</span><span class="sxs-lookup"><span data-stu-id="b6801-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="b6801-104">Para saber mais sobre esses limites, confira [aqui](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="b6801-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="b6801-105">Para desencorajar a entrega de mensagens não solicitadas em massa, aplicamos **limites de taxa de destinatário por usuário a todas as mensagens de saída e internas**.</span><span class="sxs-lookup"><span data-stu-id="b6801-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="b6801-106">Em todas as SKUs, esse limite é de **10.000 destinatários por dia**.</span><span class="sxs-lookup"><span data-stu-id="b6801-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="b6801-107">Os clientes que precisam enviar emails comerciais legítimos em massa (por exemplo, boletins informativos para clientes) devem usar provedores de terceiros especializados nesses serviços.</span><span class="sxs-lookup"><span data-stu-id="b6801-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="b6801-108">**Observação**: Após o limite ter sido atingido, não será mais possível enviar mensagens da caixa de correio até que o número de destinatários para os quais foram enviadas mensagens nas últimas 24 horas fique abaixo do limite.</span><span class="sxs-lookup"><span data-stu-id="b6801-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="b6801-109">O usuário não poderá enviar mensagens até esse ponto.</span><span class="sxs-lookup"><span data-stu-id="b6801-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="b6801-110">A taxa limite de mensagem de **30 mensagens por minuto** são aplicadas a todas as SKUs.</span><span class="sxs-lookup"><span data-stu-id="b6801-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="b6801-111">Isso determina quantas mensagens um usuário pode enviar de suas contas do Exchange Online dentro de um período especificado.</span><span class="sxs-lookup"><span data-stu-id="b6801-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="b6801-112">O **número máximo de destinatários permitidos nos campos Para, CC e CCO** para uma única mensagem de email, em todas as SKUs, é **1000 destinatários**.</span><span class="sxs-lookup"><span data-stu-id="b6801-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="b6801-113">Para personalizar esse limite, veja [aqui](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="b6801-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>

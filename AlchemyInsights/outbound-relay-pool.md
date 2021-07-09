---
title: Pool de retransmissão de saída
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339950"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="ddd1f-102">Pool de retransmissão de saída</span><span class="sxs-lookup"><span data-stu-id="ddd1f-102">Outbound relay pool</span></span>

<span data-ttu-id="ddd1f-103">A Microsoft está fazendo algumas alterações na configuração para retransmitir ou encaminhar emails por meio Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="ddd1f-104">As mensagens em determinados cenários são encaminhadas ou retransmitida por Microsoft 365 usando um pool de retransmissão especial.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="ddd1f-105">As mensagens enviadas usando o pool de retransmissão podem acabar na pasta lixo eletrônico do destinatário.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="ddd1f-106">Para obter mais informações, consulte [Pools de entrega de saída](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="ddd1f-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="ddd1f-107">Para evitar um cenário usando o pool de retransmissão, certifique-se de que as mensagens encaminhadas/retransmitida atendem a um dos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="ddd1f-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="ddd1f-108">O remetente de saída é um domínio aceito do locatário.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="ddd1f-109">A Estrutura de Política de Remetente (SPF) passa quando a mensagem é Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="ddd1f-110">DomainKeys Identified Mail (DKIM) no domínio de remetente P2 passa quando a mensagem é Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="ddd1f-111">As mensagens que atendem aos critérios acima não são retransmitidas pelo pool de retransmissão.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="ddd1f-112">Se o registro MX do seu domínio for apontado para um servidor local ou de terceiros, use filtragem aprimorada para garantir que a validação SPF está correta para email de entrada e para evitar o envio de emails pelo pool de retransmissão.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="ddd1f-113">**Como saber se somos afetados pelo pool de retransmissão?**</span><span class="sxs-lookup"><span data-stu-id="ddd1f-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="ddd1f-114">Se seus emails encaminhados ou retransmitido usarem um dos critérios acima, as mensagens não serão retransmitida pelo pool de retransmissão.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="ddd1f-115">No entanto, se uma mensagem for enviada por meio de um pool de retransmissão, o IP do servidor de saída está no intervalo 40.95.0.0/16 e o nome do servidor de saída inclui **rly** no nome.</span><span class="sxs-lookup"><span data-stu-id="ddd1f-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>


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
# <a name="outbound-relay-pool"></a>Pool de retransmissão de saída

A Microsoft está fazendo algumas alterações na configuração para retransmitir ou encaminhar emails por meio Microsoft 365. As mensagens em determinados cenários são encaminhadas ou retransmitida por Microsoft 365 usando um pool de retransmissão especial. As mensagens enviadas usando o pool de retransmissão podem acabar na pasta lixo eletrônico do destinatário. Para obter mais informações, consulte [Pools de entrega de saída](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Para evitar um cenário usando o pool de retransmissão, certifique-se de que as mensagens encaminhadas/retransmitida atendem a um dos seguintes critérios:

- O remetente de saída é um domínio aceito do locatário.
- A Estrutura de Política de Remetente (SPF) passa quando a mensagem é Microsoft 365.
- DomainKeys Identified Mail (DKIM) no domínio de remetente P2 passa quando a mensagem é Microsoft 365.
 
As mensagens que atendem aos critérios acima não são retransmitidas pelo pool de retransmissão.

Se o registro MX do seu domínio for apontado para um servidor local ou de terceiros, use filtragem aprimorada para garantir que a validação SPF está correta para email de entrada e para evitar o envio de emails pelo pool de retransmissão.

**Como saber se somos afetados pelo pool de retransmissão?**

Se seus emails encaminhados ou retransmitido usarem um dos critérios acima, as mensagens não serão retransmitida pelo pool de retransmissão. No entanto, se uma mensagem for enviada por meio de um pool de retransmissão, o IP do servidor de saída está no intervalo 40.95.0.0/16 e o nome do servidor de saída inclui **rly** no nome.


---
title: Verifique se há endereços de encaminhamento em caixas de correio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403299"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Verifique se há endereços de encaminhamento em caixas de correio

Às vezes, os hackers encaminham as mensagens de email dos usuários para si mesmos, então primeiro verificaremos se há endereços e regras de encaminhamento na caixa de correio. Em seguida, verificaremos os logs de auditoria. Veja como verificar se há endereços de encaminhamento:

1. Selecione **Usuários**  >  **Usuários ativos**.
1. Selecione o usuário cuja conta foi comprometida.
1. No sobrevoo exibido, expanda **Configurações de Email** e clique em **Editar** para Encaminhamento **de Email.**
1. Remova os endereços de encaminhamento que você não reconhece.
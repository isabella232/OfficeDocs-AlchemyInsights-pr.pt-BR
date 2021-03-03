---
title: Verifique se há endereços de encaminhamento em caixas de correio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416888"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Verifique se há endereços de encaminhamento em caixas de correio

Às vezes, os hackers encaminham as mensagens de email dos usuários para si mesmos, então primeiro verificaremos se há endereços e regras de encaminhamento na caixa de correio. Em seguida, verificaremos os logs de auditoria. Veja como verificar se há endereços de encaminhamento:

1. Selecione **Usuários**  >  **Usuários ativos**.
1. Selecione o usuário cuja conta foi comprometida.
1. No sobrevoo exibido, expanda **Configurações de Email** e clique em **Editar** para Encaminhamento **de Email.**
1. Remova os endereços de encaminhamento que você não reconhece.
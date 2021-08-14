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
ms.openlocfilehash: a67305ed92e181f0ddfc5a929e8fe9631ceefdc99dea34118bc99975461f3868
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005798"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Verifique se há endereços de encaminhamento em caixas de correio

Às vezes, os hackers encaminham as mensagens de email dos usuários para si mesmos, então primeiro verificaremos se há endereços e regras de encaminhamento na caixa de correio. Em seguida, verificaremos os logs de auditoria. Veja como verificar se há endereços de encaminhamento:

1. Selecione **Usuários**  >  **Usuários ativos**.
1. Selecione o usuário cuja conta foi comprometida.
1. No sobrevoo exibido, expanda **Mail Configurações** e clique em **Editar** para Encaminhamento **de email.**
1. Remova os endereços de encaminhamento que você não reconhece.
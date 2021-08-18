---
title: AggregateGroupMailbox full NDR recebido para email enviado para Microsoft 365 grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315898"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox full NDR recebido para email enviado para Microsoft 365 grupo

Use o seguinte comando do Shell do EXO para criar uma regra de transporte Exchange para soltar silenciosamente emails enviados para a caixa de correio de grupo agregada:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Observação**: Substitua o endereço SMTP em **-SentTo por** endereço SMTP da caixa de correio de grupo agregada em seu locatário. Você pode obter o endereço SMTP da caixa de correio de grupo agregado da NDR recebida.




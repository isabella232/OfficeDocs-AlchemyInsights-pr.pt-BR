---
title: Erro ao enviar emails bloqueados pelo SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813712"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erro ao enviar email: host do cliente bloqueado usando Spamhaus

O endereço IP que enviou a mensagem está em uma lista de bloqueios de [propriedade de Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Os motivos para serem bloqueados pelo Spamhaus incluem contas comprometidas, máquinas comprometidas que compartilham um endereço IP público e políticas de Provedor de Serviços de Internet (ISP). As correções possíveis são:
  
- Para mensagens de entrada bloqueadas em que você controla o servidor de email de origem, você precisa determinar a causa e remover o bloco do site Spamhaus.

- Para mensagens de entrada bloqueadas em que o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site Spamhaus. Se o endereço IP estiver na Lista de Bloqueios de Política (PBL), o proprietário poderá atribuir um endereço IP estático diferente ou remover o endereço do PBL.

- Para mensagens de saída bloqueadas de seu domínio conectado à Microsoft, você pode receber esse erro se as mensagens são roteadas por meio de um serviço de terceiros. Você pode usar uma ferramenta de análise WHOIS para encontrar o proprietário do endereço IP bloqueado.

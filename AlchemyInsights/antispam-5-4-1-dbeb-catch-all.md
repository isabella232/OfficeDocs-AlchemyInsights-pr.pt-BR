---
title: 5.4.1 DBEB de AntiSpam catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672421"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Correção de problemas de entrega do código de erro 550 5.4.1 acesso de retransmissão negado

Esse problema ocorre ao [verificar se um endereço de email é válido para evitar o bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede do Office 365. Tente o seguinte:

1. Determine se o problema é específico de um domínio inteiro ou de um único endereço de email:
    - Domínio inteiro: às vezes, o domínio precisa ser sincronizado; Tente [definir o domínio como interno e, em seguida, novamente como autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Endereço de email único: às vezes, o endereço precisa ser sincronizado; alterar o endereço de proxy SMTP e alterá-lo novamente pode ajudar.
2. Determinar se o problema é específico para um grupo ou uma pasta pública. Para alguns tipos de objeto, os objetos talvez precisem ser criados manualmente no Azure Active Directory.

Se você precisar de mais ajuda, abra um tíquete de suporte e especifique o escopo do problema (includidng o tipo de objeto que você está enviando) para que possamos ajudá-lo melhor.
---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821435"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corrigir problemas de entrega para o código de erro 550 5.4.1 Acesso de Retransmissão negado

Esse problema ocorre ao verificar se um endereço de email é válido para evitar [retornos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede da Microsoft. Tente o seguinte:

1. Determine se o problema é específico para um domínio inteiro ou um único endereço de email:
    - Domínio inteiro: às vezes, o domínio precisa ser sincronizado; tente [definir o domínio como Interno e volte para Autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Endereço de email único: às vezes, o endereço precisa ser sincronizado; alterar o endereço proxy smtp e, em seguida, alterar ele de volta pode ajudar.
2. Determine se o problema é específico para um grupo ou pasta pública. Para alguns tipos de objeto, os objetos podem precisar ser criados manualmente no Azure Active Directory.

Se você precisar de ajuda adicional, abra um tíquete de suporte e especifique o escopo do problema (incluindo o tipo de objeto para o qual você está enviando) para que possamos ajudá-lo melhor.
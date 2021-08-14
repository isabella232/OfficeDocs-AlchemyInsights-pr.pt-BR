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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932265"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corrigir problemas de entrega para o código de erro 550 5.4.1 Acesso de Retransmissão negado

Esse problema ocorre ao verificar se um endereço de email é válido para evitar [retornos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede da Microsoft. Tente o seguinte:

1. Determine se o problema é específico para um domínio inteiro ou um único endereço de email:
    - Domínio inteiro: às vezes, o domínio precisa ser sincronizado; tente [definir o domínio como Interno e volte para Autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Endereço de email único: às vezes, o endereço precisa ser sincronizado; alterar o endereço proxy smtp e, em seguida, alterar ele de volta pode ajudar.
2. Determine se o problema é específico para um grupo ou pasta pública. Para alguns tipos de objeto, os objetos podem precisar ser criados manualmente Azure Active Directory.

Se você precisar de ajuda adicional, abra um tíquete de suporte e especifique o escopo do problema (incluindo o tipo de objeto para o qual você está enviando) para que possamos ajudá-lo melhor.
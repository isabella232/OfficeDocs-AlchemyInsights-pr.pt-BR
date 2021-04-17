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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="7d0b7-102">Corrigir problemas de entrega para o código de erro 550 5.4.1 Acesso de Retransmissão negado</span><span class="sxs-lookup"><span data-stu-id="7d0b7-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="7d0b7-103">Esse problema ocorre ao verificar se um endereço de email é válido para evitar [retornos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7d0b7-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="7d0b7-104">Tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="7d0b7-104">Try the following:</span></span>

1. <span data-ttu-id="7d0b7-105">Determine se o problema é específico para um domínio inteiro ou um único endereço de email:</span><span class="sxs-lookup"><span data-stu-id="7d0b7-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="7d0b7-106">Domínio inteiro: às vezes, o domínio precisa ser sincronizado; tente [definir o domínio como Interno e volte para Autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="7d0b7-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="7d0b7-107">Endereço de email único: às vezes, o endereço precisa ser sincronizado; alterar o endereço proxy smtp e, em seguida, alterar ele de volta pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="7d0b7-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="7d0b7-108">Determine se o problema é específico para um grupo ou pasta pública.</span><span class="sxs-lookup"><span data-stu-id="7d0b7-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="7d0b7-109">Para alguns tipos de objeto, os objetos podem precisar ser criados manualmente no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7d0b7-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="7d0b7-110">Se você precisar de ajuda adicional, abra um tíquete de suporte e especifique o escopo do problema (incluindo o tipo de objeto para o qual você está enviando) para que possamos ajudá-lo melhor.</span><span class="sxs-lookup"><span data-stu-id="7d0b7-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>
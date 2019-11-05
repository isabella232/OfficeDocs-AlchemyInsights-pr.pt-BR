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
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964047"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="1c62d-102">Correção de problemas de entrega do código de erro 550 5.4.1 acesso de retransmissão negado</span><span class="sxs-lookup"><span data-stu-id="1c62d-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="1c62d-103">Esse problema ocorre ao [verificar se um endereço de email é válido para evitar o bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1c62d-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="1c62d-104">Tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="1c62d-104">Try the following:</span></span>

1. <span data-ttu-id="1c62d-105">Determine se o problema é específico de um domínio inteiro ou de um único endereço de email:</span><span class="sxs-lookup"><span data-stu-id="1c62d-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="1c62d-106">Domínio inteiro: às vezes, o domínio precisa ser sincronizado; Tente [definir o domínio como interno e, em seguida, novamente como autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="1c62d-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="1c62d-107">Endereço de email único: às vezes, o endereço precisa ser sincronizado; alterar o endereço de proxy SMTP e alterá-lo novamente pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="1c62d-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="1c62d-108">Determinar se o problema é específico para um grupo ou uma pasta pública.</span><span class="sxs-lookup"><span data-stu-id="1c62d-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="1c62d-109">Para alguns tipos de objeto, os objetos talvez precisem ser criados manualmente no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1c62d-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="1c62d-110">Se você precisar de mais ajuda, abra um tíquete de suporte e especifique o escopo do problema (includidng o tipo de objeto que você está enviando) para que possamos ajudá-lo melhor.</span><span class="sxs-lookup"><span data-stu-id="1c62d-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>
---
title: 5.4.1 DBEB de AntiSpam catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717349"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="d0893-102">Correção de problemas de entrega do código de erro 550 5.4.1 acesso de retransmissão negado</span><span class="sxs-lookup"><span data-stu-id="d0893-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="d0893-103">Esse problema ocorre ao [verificar se um endereço de email é válido para evitar o bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d0893-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="d0893-104">Tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d0893-104">Try the following:</span></span>

1. <span data-ttu-id="d0893-105">Determine se o problema é específico de um domínio inteiro ou de um único endereço de email:</span><span class="sxs-lookup"><span data-stu-id="d0893-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="d0893-106">Domínio inteiro: às vezes, o domínio precisa ser sincronizado; Tente [definir o domínio como interno e, em seguida, novamente como autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="d0893-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="d0893-107">Endereço de email único: às vezes, o endereço precisa ser sincronizado; alterar o endereço de proxy SMTP e alterá-lo novamente pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="d0893-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="d0893-108">Determinar se o problema é específico para um grupo ou uma pasta pública.</span><span class="sxs-lookup"><span data-stu-id="d0893-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="d0893-109">Para alguns tipos de objeto, os objetos talvez precisem ser criados manualmente no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0893-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="d0893-110">Se você precisar de mais ajuda, abra um tíquete de suporte e especifique o escopo do problema (incluindo o tipo de objeto que você está enviando) para que possamos ajudá-lo melhor.</span><span class="sxs-lookup"><span data-stu-id="d0893-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>
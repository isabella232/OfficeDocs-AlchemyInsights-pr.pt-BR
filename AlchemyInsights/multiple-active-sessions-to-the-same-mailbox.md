---
title: Várias sessões ativas para a mesma caixa de correio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769711"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="51e01-102">Várias sessões ativas para a mesma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="51e01-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="51e01-103">Para controlar o uso de recursos do Exchange, uma caixa de correio do tem um "orçamento".</span><span class="sxs-lookup"><span data-stu-id="51e01-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="51e01-104">A exceção acima do orçamento pode ser disparada por, mas não está limitada a, as seguintes circunstâncias:</span><span class="sxs-lookup"><span data-stu-id="51e01-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="51e01-105">Algumas guias do navegador são abertas dentro da mesma sessão do aplicativo Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="51e01-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="51e01-106">Algumas sessões ativas do Outlook Web App para a mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="51e01-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="51e01-107">Alguns outros aplicativos de cliente (Outlook, Outlook Mobile, um aplicativo de cliente de terceiros) acessam a caixa de correio ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="51e01-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="51e01-108">Operações de longa duração, como executar solicitações de pesquisa, são realizadas em outra sessão de caixa de correio ativa.</span><span class="sxs-lookup"><span data-stu-id="51e01-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>


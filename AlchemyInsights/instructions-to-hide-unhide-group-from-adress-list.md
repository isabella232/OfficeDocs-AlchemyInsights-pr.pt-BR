---
title: Instruções para ocultar/reexibir grupo da lista de endereços
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908332"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="b5ba0-102">Ocultar o Microsoft 365 Group da lista de endereços (GAL)</span><span class="sxs-lookup"><span data-stu-id="b5ba0-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="b5ba0-103">Para ocultar um grupo do Microsoft 365 de listas de endereços (GAL) de clientes do Exchange (como Outlook ou OWA), use o seguinte comando no Shell do EXO:</span><span class="sxs-lookup"><span data-stu-id="b5ba0-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="b5ba0-104">Para ocultar o grupo Microsoft 365 de ser visível para os clientes do Exchange, use o seguinte comando no Shell do EXO:</span><span class="sxs-lookup"><span data-stu-id="b5ba0-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


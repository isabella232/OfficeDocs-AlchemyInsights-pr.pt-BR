---
title: Pasta pública habilitada para enviar como email no EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451378"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="f8472-102">Pasta pública de sendas habilitada para email</span><span class="sxs-lookup"><span data-stu-id="f8472-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="f8472-103">O exemplo a seguir atribui permissões "Send as" para a pasta pública habilitada para email NewPF1 para o usuário Jason.</span><span class="sxs-lookup"><span data-stu-id="f8472-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="f8472-104">Add-RecipientPermission-Identity ' NewPF1 '-trustee "Jason"-AccessRights ' sendas '</span><span class="sxs-lookup"><span data-stu-id="f8472-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="f8472-105">Para informações detalhadas de sintaxes e de parâmetros, consulte [atribuir permissões "enviar como" ou "enviar em nome" para pastas públicas habilitadas para email](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="f8472-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>


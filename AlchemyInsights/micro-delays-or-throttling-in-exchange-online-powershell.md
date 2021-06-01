---
title: Micro atrasos ou limitação no Windows PowerShell do Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702114"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="26458-102">Micro atrasos ou limitação no Windows PowerShell do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="26458-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="26458-103">É provável que você veja os avisos "Ocorreram micro atrasos" ou os atrasos executar scripts e cmdlets no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="26458-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="26458-104">Eis algumas sugestões de como resolver isso: </span><span class="sxs-lookup"><span data-stu-id="26458-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="26458-105">Execute nossos diagnósticos para relaxar as políticas de locação do PowerShell do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="26458-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="26458-106">Essa solução resolverá o problema para a maioria.</span><span class="sxs-lookup"><span data-stu-id="26458-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="26458-107">Se o problema ainda não tiver sido resolvido, use o [Módulo do PowerShell no Exchange Online v2](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), que inclui CMDlets baseados na API REST e que são significativamente mais eficazes.</span><span class="sxs-lookup"><span data-stu-id="26458-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="26458-108">Essa pode ser uma ótima solução para muitos CMDlets de Get- que são usados com frequência.</span><span class="sxs-lookup"><span data-stu-id="26458-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="26458-109">Se você precisar usar CMDlets que não são abordados no módulo v2, consulte [Executando cmdlets do PowerShell para grandes quantidades de usuários no Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que tratam de como conferir os limites esperados de limitação do PowerShell no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="26458-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>

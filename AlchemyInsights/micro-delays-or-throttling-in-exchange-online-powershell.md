---
title: Micro atrasos ou limitação no Windows PowerShell do Exchange Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743844"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="cf7dd-102">Micro atrasos ou limitação no Windows PowerShell do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="cf7dd-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="cf7dd-103">É provável que você veja os avisos "Ocorreram micro atrasos" ou os atrasos executar scripts e cmdlets no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="cf7dd-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="cf7dd-104">Aqui estão duas sugestões relacionadas a isso:</span><span class="sxs-lookup"><span data-stu-id="cf7dd-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="cf7dd-105">Talvez você queira tentar usar o [módulo Exchange Online v2 do Windows PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), que inclui CMDlets baseados na API REST e são muito mais eficazes.</span><span class="sxs-lookup"><span data-stu-id="cf7dd-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="cf7dd-106">Pode ser uma ótima solução para muitos CMDlets de Get que são usados com frequência.</span><span class="sxs-lookup"><span data-stu-id="cf7dd-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="cf7dd-107">Se você precisar usar CMDlets que não são abordados no módulo v2 ainda, confira [Executando cmdlets do PowerShell para grandes quantidades de usuários no Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que fala sobre como conferir os limites esperados de limitação do Windows PowerShell no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="cf7dd-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>

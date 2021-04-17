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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830021"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro atrasos ou limitação no Windows PowerShell do Exchange Online

É provável que você veja os avisos "Ocorreram micro atrasos" ou os atrasos executar scripts e cmdlets no Exchange Online. Aqui estão duas sugestões relacionadas a isso:

- Talvez você queira tentar usar o [módulo Exchange Online v2 do Windows PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), que inclui CMDlets baseados na API REST e são muito mais eficazes. Pode ser uma ótima solução para muitos CMDlets de Get que são usados com frequência.
- Se você precisar usar CMDlets que não são abordados no módulo v2 ainda, confira [Executando cmdlets do PowerShell para grandes quantidades de usuários no Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que fala sobre como conferir os limites esperados de limitação do Windows PowerShell no Exchange Online.

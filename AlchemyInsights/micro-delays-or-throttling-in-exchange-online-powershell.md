---
title: Micro atrasos ou limitação no Windows PowerShell do Exchange Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947769"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro atrasos ou limitação no Windows PowerShell do Exchange Online

É provável que você veja os avisos "Ocorreram micro atrasos" ou os atrasos executar scripts e cmdlets no Exchange Online. Aqui estão duas sugestões relacionadas a isso:

- Talvez você queira tentar usar o [módulo Exchange Online v2 do Windows PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), que inclui CMDlets baseados na API REST e são muito mais eficazes. Pode ser uma ótima solução para muitos CMDlets de Get que são usados com frequência.
- Se você precisar usar CMDlets que não são abordados no módulo v2 ainda, confira [Executando cmdlets do PowerShell para grandes quantidades de usuários no Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que fala sobre como conferir os limites esperados de limitação do Windows PowerShell no Exchange Online.

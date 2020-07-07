---
title: Mensagens enviadas para o grupo Microsoft 365 não são recebidas por todos os membros
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2020
ms.locfileid: "45047227"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Mensagens enviadas para o grupo Microsoft 365 não são recebidas por todos os membros

Certifique-se de que todos os membros do grupo se inscreveram para receber os emails. Confira [acompanhar um grupo no Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Para verificar o status da mensagem dos membros que se inscreveram em emails do grupo, execute o seguinte comando no [EXO do PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`
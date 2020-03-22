---
title: Não é possível acessar pastas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891737"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>O Outlook não consegue se conectar a pastas públicas

Se o acesso à pasta pública não estiver funcionando para alguns usuários, tente o seguinte:

Conecte-se ao EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de usuário com problema para corresponder ao parâmetro em uma conta de usuário em funcionamento.

Exemplo:

Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valor de comando anterior>

Aguarde pelo menos uma hora para que a alteração entre em vigor.

Se o problema permanecer, siga [este procedimento](https://aka.ms/pfcte) para solucionar problemas de acesso à pasta pública usando o Outlook.
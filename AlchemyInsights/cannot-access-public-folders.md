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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959483"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>O Outlook não consegue se conectar a pastas públicas

Se o acesso à pasta pública não estiver funcionando para alguns usuários, tente o seguinte:

Conecte-se ao EXO PowerShell e configure o DefaultPublicFolderMailbox na conta de usuário com problema para corresponder a um em uma conta de usuário em funcionamento.

Exemplo:

Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valor de comando anterior>

Aguarde pelo menos uma hora para que a alteração entre em vigor.
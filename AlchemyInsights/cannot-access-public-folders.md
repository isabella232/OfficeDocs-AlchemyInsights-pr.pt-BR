---
title: Não é possível acessar pastas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812535"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>O Outlook não consegue se conectar a pastas públicas

Se o acesso à pasta pública não estiver funcionando para alguns usuários, tente o seguinte:

Conecte-se ao EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de usuário com problema para corresponder ao parâmetro em uma conta de usuário em funcionamento.

Exemplo:

Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Aguarde pelo menos uma hora para que a alteração entre em vigor.

Se o problema permanecer, siga [este procedimento](https://aka.ms/pfcte) para solucionar problemas de acesso à pasta pública usando o Outlook.
 
**Para controlar quais usuários podem acessar pastas públicas usando o Outlook**:

1.  Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true: permitir que os usuários acessem pastas públicas no Outlook  
      
    $false: impedir que os usuários acessem pastas públicas no Outlook. Esse é o valor padrão.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Observação** Este procedimento só pode controlar conexões com o Outlook desktop para clientes Windows. Um usuário pode continuar acessando pastas públicas usando o OWA ou o Outlook para Mac.
 
Para obter mais informações, consulte [anunciando suporte para conexões controladas para pastas públicas no Outlook](https://aka.ms/controlpf).
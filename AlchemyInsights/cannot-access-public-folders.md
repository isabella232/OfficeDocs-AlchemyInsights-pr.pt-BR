---
title: Não é possível acessar pastas públicas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996618"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook não pode se conectar a pastas públicas

Se o acesso a pastas públicas não estiver funcionando para alguns usuários, tente o seguinte:

Conexão o EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de usuário do problema para corresponder ao parâmetro em uma conta de usuário funcionando.

Exemplo:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Aguarde pelo menos uma hora para que a alteração entre em vigor.

Se o problema permanecer, siga [este](https://aka.ms/pfcte) procedimento para solucionar problemas de acesso a pastas públicas usando Outlook.
 
**Para controlar quais usuários podem acessar pastas públicas usando Outlook**:

1.  Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true: permitir que os usuários acessem pastas públicas no Outlook  
      
    $false: impedir que os usuários acessem pastas públicas no Outlook. Esse é o valor padrão.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Observação** Este procedimento só pode controlar conexões com Outlook desktop para Windows clientes. Um usuário pode continuar acessando pastas públicas usando o OWA ou Outlook para Mac.
 
Para obter mais informações, consulte [Anunciando o suporte para conexões controladas com](https://aka.ms/controlpf)pastas públicas em Outlook .
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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819500"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>O Outlook não pode se conectar a pastas públicas

Se o acesso a pastas públicas não estiver funcionando para alguns usuários, tente o seguinte:

Conecte-se ao EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de usuário do problema para corresponder ao parâmetro em uma conta de usuário funcionando.

Exemplo:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Aguarde pelo menos uma hora para que a alteração entre em vigor.

Se o problema permanecer, siga este procedimento [para](https://aka.ms/pfcte) solucionar problemas de acesso a pastas públicas usando o Outlook.
 
**Para controlar quais usuários podem acessar pastas públicas usando o Outlook**:

1.  Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true: permitir que os usuários acessem pastas públicas no Outlook  
      
    $false: impedir que os usuários acessem pastas públicas no Outlook. Esse é o valor padrão.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Observação** Esse procedimento só pode controlar conexões com a área de trabalho do Outlook para clientes Windows. Um usuário pode continuar acessando pastas públicas usando o OWA ou o Outlook para Mac.
 
Para obter mais informações, consulte [Anunciando o suporte para conexões controladas com pastas públicas no Outlook](https://aka.ms/controlpf).
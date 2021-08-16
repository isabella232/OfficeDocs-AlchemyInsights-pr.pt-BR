---
title: Controlar o acesso às pastas públicas usando o Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032546"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlar o acesso às pastas públicas usando o Outlook

Para controlar quais usuários podem acessar pastas públicas usando o Outlook:

1. Usar o `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: permitir que os usuários acessem pastas públicas no Outlook  
$false: impedir que os usuários acessem pastas públicas no Outlook. Esse é o valor padrão.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Observação: este procedimento pode controlar somente as conexões com a área de trabalho do Outlook para clientes Windows. Os usuários podem continuar acessando as pastas públicas usando o OWA ou o Outlook para Mac.

Para saber mais, confira [Conexões controladas para pastas públicas no Outlook](https://aka.ms/controlpf).

---
title: Controlar o acesso às pastas públicas usando o Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406531"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlar o acesso às pastas públicas usando o Outlook

Para controlar quais usuários podem acessar pastas públicas usando o Outlook:

1. Usar o `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: permitir que os usuários acessem pastas públicas no Outlook  
$false: impedir que os usuários acessem pastas públicas no Outlook. Esse é o valor padrão.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Observação: este procedimento pode controlar somente as conexões com a área de trabalho do Outlook para clientes Windows. Os usuários podem continuar acessando as pastas públicas usando o OWA ou o Outlook para Mac.

Para saber mais, confira [Conexões controladas para pastas públicas no Outlook](https://aka.ms/controlpf).

---
title: Controlar o acesso às pastas públicas usando o Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680446"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlar o acesso às pastas públicas usando o Outlook

Para controlar quais usuários podem acessar pastas públicas usando o Outlook:

1. Usar o `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: permitir que os usuários acessem pastas públicas no Outlook  
$false: impedir que os usuários acessem pastas públicas no Outlook. Esse é o valor padrão.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Observação: este procedimento pode controlar somente as conexões com a área de trabalho do Outlook para clientes Windows. Os usuários podem continuar acessando as pastas públicas usando o OWA ou o Outlook para Mac.

Para saber mais, confira [Conexões controladas para pastas públicas no Outlook](https://aka.ms/controlpf).

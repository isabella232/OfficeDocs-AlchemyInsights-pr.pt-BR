---
title: O proprietário não consegue criar subpasta usando o Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716506"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>O proprietário não consegue criar subpasta usando o Outlook

**Há um problema contínuo com os proprietários de pasta pública que criam subpastas usando o Outlook. O problema será corrigido em breve.**

Você pode usar uma das seguintes soluções alternativas:

1. Use o Outlook para MAC para criar a subpasta, já que o problema afeta apenas o Outlook para Windows para área de trabalho (todas as versões)
2. O administrador cria a subpasta usando o Shell EXO ou o EAC
3. Alterar o DefaultPublicFolderMailbox/EffectivePublicFolderMailbox no usuário para outra caixa de correio do que a caixa de correio de conteúdo da pasta, causando o problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Esperar por uma hora, reiniciar o cliente do Outlook
---
title: Permissões de calendário
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046092"
---
# <a name="calendar-permissions"></a>Permissões de calendário

Os usuários podem alterar suas próprias Permissões de Calendário com Outlook na Web ou em outros clientes, mas, como administrador, talvez seja necessário investigar também.  
Com Exchange cmdlet do PowerShell mostrará a permissão no calendário de um usuário:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Para ver mais informações, consulte o seguinte:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Permissões de calendário são usadas no compartilhamento de calendários, para ver mais informações sobre o compartilhamento Outlook calendário, consulte estes artigos:

- [Compartilhar um calendário do Outlook com outras pessoas ](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Compartilhar seu calendário no Outlook na Web para empresas](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Para solucionar problemas de Permissão de Calendário, você pode usar a [Assistente de Recuperação e Suporte](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) ferramenta.
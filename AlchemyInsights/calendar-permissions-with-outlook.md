---
title: Permissões de calendário
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44853974"
---
# <a name="calendar-permissions"></a>Permissões de calendário

Os usuários podem alterar suas próprias permissões de calendário com o Outlook na Web ou outros clientes, mas como um administrador também pode ser necessário investigar.  
Com o cmdlet do Exchange PowerShell lhe mostrará a permissão no calendário de um usuário:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Para ver mais informações, consulte o seguinte:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

As permissões de calendário são usadas no compartilhamento de calendários para ver mais informações sobre como compartilhar um calendário do Outlook, consulte estes artigos:

- [Compartilhar um calendário do Outlook com outras pessoas](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Compartilhar seu calendário no Outlook na Web para empresas](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Para solucionar problemas de calendário, você pode usar a ferramenta de [Assistente de recuperação e suporte](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .
---
title: Ausência de emails em quarentena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542073"
---
# <a name="missing-emails-in-quarantine"></a>Emails ausentes em quarentena "

Os administradores podem [Exibir, liberar ou excluir essas mensagens.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Para abrir o centro de conformidade & segurança, vá para [https://protection.office.com](https://protection.office.com/) . Para abrir a página de quarentena diretamente, acesse [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Você pode pesquisar pelos seguintes valores:  

- **ID da mensagem**: o identificador globalmente exclusivo da mensagem. Se você selecionar uma mensagem na lista, o valor **ID da mensagem** aparecerá no painel de submenu **detalhes** exibido. Os administradores podem usar [Rastreamento da mensagem](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para localizar mensagens e seus valores da ID da mensagem correspondentes.
- **Endereço de e-mail do remetente**: o endereço de e-mail de um único remetente.
- **Endereço de e-mail do destinatário**: o endereço de e-mail de um único destinatário.
- **Assunto**: use todo o assunto da mensagem. A pesquisa não diferencia maiúsculas de minúsculas.

Depois de inserir os critérios de pesquisa, clique em ![ Atualizar botão ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atualizar** para filtrar os resultados.  

Os cmdlets que você usa para exibir e gerenciar mensagens e arquivos em quarentena são:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Observe que este cmdlet é somente para mensagens, e não para arquivos de malware de ATP para SharePoint Online, onedrive for Business ou Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
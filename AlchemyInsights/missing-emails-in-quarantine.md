---
title: Emails ausentes em quarentena
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
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831722"
---
# <a name="missing-emails-in-quarantine"></a>Emails ausentes em quarentena"

Os administradores [podem exibir, liberar ou excluir essas mensagens.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Para abrir o Centro de Conformidade & segurança, vá para [https://protection.office.com](https://protection.office.com/) . Para abrir a página Quarentena diretamente, vá para [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Você pode pesquisar pelos seguintes valores:  

- **ID da mensagem**: o identificador globalmente exclusivo da mensagem. Se você selecionar uma mensagem na lista, o  valor **de ID** da mensagem será exibido no painel Detalhes do flyout que aparece. Os administradores podem usar [Rastreamento da mensagem](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para localizar mensagens e seus valores da ID da mensagem correspondentes.
- **Endereço de e-mail do remetente**: o endereço de e-mail de um único remetente.
- **Endereço de e-mail do destinatário**: o endereço de e-mail de um único destinatário.
- **Assunto**: use todo o assunto da mensagem. A pesquisa não diferencia maiúsculas de minúsculas.

Depois de ter inserido os critérios de pesquisa, clique em Atualizar botão ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atualizar** para filtrar os resultados.  

Os cmdlets que você usa para exibir e gerencia mensagens e arquivos em quarentena são:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): observe que esse cmdlet é apenas para mensagens, não arquivos de malware da ATP para SharePoint Online, OneDrive for Business ou Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
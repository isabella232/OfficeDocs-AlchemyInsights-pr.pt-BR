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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026210"
---
# <a name="missing-emails-in-quarantine"></a>Emails ausentes em quarentena"

Os administradores [podem exibir, liberar ou excluir essas mensagens.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Para abrir o Centro de Conformidade & segurança, vá para [https://protection.office.com](https://protection.office.com/) . Para abrir a página Quarentena diretamente, vá para [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Você pode pesquisar pelos seguintes valores:  

- **ID da mensagem**: o identificador globalmente exclusivo da mensagem. Se você selecionar uma mensagem na lista, o  valor **de ID** da mensagem será exibido no painel Detalhes do flyout que aparece. Os administradores podem usar [Rastreamento da mensagem](/microsoft-365/security/office-365-security/message-trace-scc) para localizar mensagens e seus valores da ID da mensagem correspondentes.
- **Endereço de e-mail do remetente**: o endereço de e-mail de um único remetente.
- **Endereço de e-mail do destinatário**: o endereço de e-mail de um único destinatário.
- **Assunto**: use todo o assunto da mensagem. A pesquisa não diferencia maiúsculas de minúsculas.

Depois de ter inserido os critérios da pesquisa, clique em ![Atualizar botão](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atualizar** para filtrar os resultados.

Os cmdlets que você usa para exibir e gerencia mensagens e arquivos em quarentena são:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): observe que esse cmdlet é apenas para mensagens, não arquivos de malware do Microsoft Defender para Office 365 para SharePoint Online, OneDrive for Business ou Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)
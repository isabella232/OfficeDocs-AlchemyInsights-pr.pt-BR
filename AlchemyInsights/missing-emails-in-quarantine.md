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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329650"
---
# <a name="missing-emails-in-quarantine"></a>Emails ausentes em quarentena

Os administradores podem [exibir, liberar ou excluir essas mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

No portal Microsoft 365 Defender em <https://security.microsoft.com> , vá para **Analisar** \> **Quarentena**. Ou, para ir diretamente para a página **Quarentena,** use <https://security.microsoft.com/quarantine> .  

Para obter mais informações sobre os valores de pesquisa/filtro que você pode usar, consulte [Manage quarantined messages and files as an admin in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Os cmdlets que você usa para exibir e gerencia mensagens e arquivos em quarentena são:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): observe que esse cmdlet é apenas para mensagens, não arquivos de Cofre Anexos para SharePoint, OneDrive ou Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)

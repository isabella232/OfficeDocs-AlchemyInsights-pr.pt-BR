---
title: Bloquear download em links de compartilhamento
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
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685730"
---
# <a name="block-download-on-sharing-links"></a>Bloquear download em links de compartilhamento

**Bloquear download** está disponível para **links somente para exibição** a documentos do Office. Quando você seleciona essa opção, as pessoas que recebem acesso ao arquivo por meio do link que você criou não virão as opções para baixar, imprimir ou copiar o arquivo.

Os administradores podem controlar se a configuração de "bloquear download" é exibida somente para arquivos do Office ou não alterando a `BlockDownloadLinksFileType` configuração no [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) ou [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)cmdlets do PowerShell.

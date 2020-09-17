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
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="bff95-102">Bloquear download em links de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="bff95-102">Block download on sharing links</span></span>

<span data-ttu-id="bff95-103">**Bloquear download** está disponível para **links somente para exibição** a documentos do Office.</span><span class="sxs-lookup"><span data-stu-id="bff95-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="bff95-104">Quando você seleciona essa opção, as pessoas que recebem acesso ao arquivo por meio do link que você criou não virão as opções para baixar, imprimir ou copiar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="bff95-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="bff95-105">Os administradores podem controlar se a configuração de "bloquear download" é exibida somente para arquivos do Office ou não alterando a `BlockDownloadLinksFileType` configuração no [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) ou [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)cmdlets do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bff95-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>

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
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="ee176-102">Controlar o acesso às pastas públicas usando o Outlook</span><span class="sxs-lookup"><span data-stu-id="ee176-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="ee176-103">Para controlar quais usuários podem acessar pastas públicas usando o Outlook:</span><span class="sxs-lookup"><span data-stu-id="ee176-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="ee176-104">Usar o `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="ee176-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="ee176-105">$true: permitir que os usuários acessem pastas públicas no Outlook</span><span class="sxs-lookup"><span data-stu-id="ee176-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="ee176-106">$false: impedir que os usuários acessem pastas públicas no Outlook.</span><span class="sxs-lookup"><span data-stu-id="ee176-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="ee176-107">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="ee176-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="ee176-108">Observação: este procedimento pode controlar somente as conexões com a área de trabalho do Outlook para clientes Windows.</span><span class="sxs-lookup"><span data-stu-id="ee176-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="ee176-109">Os usuários podem continuar acessando as pastas públicas usando o OWA ou o Outlook para Mac.</span><span class="sxs-lookup"><span data-stu-id="ee176-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="ee176-110">Para saber mais, confira [Conexões controladas para pastas públicas no Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="ee176-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>

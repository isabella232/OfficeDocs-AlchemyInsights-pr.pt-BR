---
title: Erro de endereço proxy ao criar uma caixa de correio compartilhada
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568278"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="d2d8c-102">Erro de endereço proxy ao criar uma caixa de correio ou outro objeto habilitado para email</span><span class="sxs-lookup"><span data-stu-id="d2d8c-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="d2d8c-103">Se você tentou criar um objeto habilitado para email (caixa de correio, caixa de correio compartilhada etc.) e recebeu o erro "O endereço proxy "SMTP:alias@domain.com" já está sendo usado...", o endereço de email escolhido já será tomado por outro objeto habilitado para email em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d2d8c-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="d2d8c-104">Você precisa encontrar o usuário, grupo, caixa de correio compartilhada ou pasta pública que tenha esse endereço de email e excluí-lo ou alterar seu endereço de email.</span><span class="sxs-lookup"><span data-stu-id="d2d8c-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="d2d8c-105">Em seguida, você pode criar um novo objeto habilitado para email com o endereço de email liberado.</span><span class="sxs-lookup"><span data-stu-id="d2d8c-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="d2d8c-106">Use a Pesquisa na Página Inicial para encontrá-la.</span><span class="sxs-lookup"><span data-stu-id="d2d8c-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="d2d8c-107">Você também pode usar o seguinte comando do PowerShell do Exchange Online para pesquisá-lo:</span><span class="sxs-lookup"><span data-stu-id="d2d8c-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="d2d8c-108">Se você não quiser excluir o endereço de email existente, escolha um novo endereço de email para o novo objeto que você está criando.</span><span class="sxs-lookup"><span data-stu-id="d2d8c-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  
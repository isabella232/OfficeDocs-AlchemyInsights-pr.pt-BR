---
title: O proprietário não consegue criar subpasta usando o Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665706"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="c7565-102">O proprietário não consegue criar subpasta usando o Outlook</span><span class="sxs-lookup"><span data-stu-id="c7565-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="c7565-103">**Há um problema contínuo com os proprietários de pasta pública que criam subpastas usando o Outlook. O problema será corrigido em breve.**</span><span class="sxs-lookup"><span data-stu-id="c7565-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="c7565-104">Você pode usar uma das seguintes soluções alternativas:</span><span class="sxs-lookup"><span data-stu-id="c7565-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="c7565-105">Use o Outlook para MAC para criar a subpasta, já que o problema afeta apenas o Outlook para Windows para área de trabalho (todas as versões)</span><span class="sxs-lookup"><span data-stu-id="c7565-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="c7565-106">O administrador cria a subpasta usando o Shell EXO ou o EAC</span><span class="sxs-lookup"><span data-stu-id="c7565-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="c7565-107">Alterar o DefaultPublicFolderMailbox/EffectivePublicFolderMailbox no usuário para outra caixa de correio do que a caixa de correio de conteúdo da pasta, causando o problema</span><span class="sxs-lookup"><span data-stu-id="c7565-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="c7565-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="c7565-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="c7565-109">Esperar por uma hora, reiniciar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="c7565-109">Wait for an hour, restart outlook client</span></span>
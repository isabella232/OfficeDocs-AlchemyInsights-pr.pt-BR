---
title: O proprietário não consegue criar subpasta usando o Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836123"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="93e66-102">O proprietário não consegue criar subpasta usando o Outlook</span><span class="sxs-lookup"><span data-stu-id="93e66-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="93e66-103">**Há um problema contínuo com os proprietários de pasta pública que criam subpastas usando o Outlook. O problema será corrigido em breve.**</span><span class="sxs-lookup"><span data-stu-id="93e66-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="93e66-104">Você pode usar uma das seguintes soluções alternativas:</span><span class="sxs-lookup"><span data-stu-id="93e66-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="93e66-105">Use o Outlook para MAC para criar a subpasta, já que o problema afeta apenas o Outlook para Windows para área de trabalho (todas as versões)</span><span class="sxs-lookup"><span data-stu-id="93e66-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="93e66-106">O administrador cria a subpasta usando o Shell EXO ou o EAC</span><span class="sxs-lookup"><span data-stu-id="93e66-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="93e66-107">Alterar o DefaultPublicFolderMailbox/EffectivePublicFolderMailbox no usuário para outra caixa de correio do que a caixa de correio de conteúdo da pasta, causando o problema</span><span class="sxs-lookup"><span data-stu-id="93e66-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="93e66-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="93e66-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="93e66-109">Esperar por uma hora, reiniciar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="93e66-109">Wait for an hour, restart outlook client</span></span>
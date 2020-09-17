---
title: Restaurar uma pasta pública excluída
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774519"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="83f3d-102">Restaurar uma pasta pública excluída</span><span class="sxs-lookup"><span data-stu-id="83f3d-102">Restore a deleted public folder</span></span>

<span data-ttu-id="83f3d-103">**Para restaurar itens excluídos de uma pasta pública**:</span><span class="sxs-lookup"><span data-stu-id="83f3d-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="83f3d-104">Confira [não é possível recuperar itens excluídos de uma pasta pública que não seja de email no Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="83f3d-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="83f3d-105">**Para restaurar uma pasta pública excluída (de qualquer tipo)**:</span><span class="sxs-lookup"><span data-stu-id="83f3d-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="83f3d-106">Use o seguinte comando do EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="83f3d-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="83f3d-107">Sintaxe:</span><span class="sxs-lookup"><span data-stu-id="83f3d-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="83f3d-108">Exemplo: o comando a seguir irá restaurar o Subfolder1 e colocá-lo em \Parent1:</span><span class="sxs-lookup"><span data-stu-id="83f3d-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="83f3d-109">Consulte [restaurar uma pasta pública excluída](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="83f3d-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>

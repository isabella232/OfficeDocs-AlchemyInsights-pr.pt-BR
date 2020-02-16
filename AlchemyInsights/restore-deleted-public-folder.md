---
title: Restaurar uma pasta pública excluída
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063586"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="b3901-102">Restaurar uma pasta pública excluída</span><span class="sxs-lookup"><span data-stu-id="b3901-102">Restore a deleted public folder</span></span>

<span data-ttu-id="b3901-103">**Para restaurar itens excluídos de uma pasta pública**:</span><span class="sxs-lookup"><span data-stu-id="b3901-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="b3901-104">Confira [não é possível recuperar itens excluídos de uma pasta pública que não seja de email no Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="b3901-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="b3901-105">**Para restaurar uma pasta pública excluída (de qualquer tipo)**:</span><span class="sxs-lookup"><span data-stu-id="b3901-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="b3901-106">Use o seguinte comando do EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b3901-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="b3901-107">Sintaxe:</span><span class="sxs-lookup"><span data-stu-id="b3901-107">Syntax:</span></span>

    ><span data-ttu-id="b3901-108">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity-Path \<caminho onde a pasta será restaurada></span><span class="sxs-lookup"><span data-stu-id="b3901-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="b3901-109">Exemplo: o comando a seguir irá restaurar o Subfolder1 e colocá-lo em \Parent1:</span><span class="sxs-lookup"><span data-stu-id="b3901-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="b3901-110">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-EQ "Subfolder1"}; Set-PublicFolder $pf. Identity-Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="b3901-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="b3901-111">Consulte [restaurar uma pasta pública excluída](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="b3901-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>

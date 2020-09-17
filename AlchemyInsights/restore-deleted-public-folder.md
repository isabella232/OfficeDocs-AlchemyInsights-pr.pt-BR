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
# <a name="restore-a-deleted-public-folder"></a>Restaurar uma pasta pública excluída

**Para restaurar itens excluídos de uma pasta pública**:

- Confira [não é possível recuperar itens excluídos de uma pasta pública que não seja de email no Outlook 2016](https://aka.ms/pfrec).
 
**Para restaurar uma pasta pública excluída (de qualquer tipo)**: 

- Use o seguinte comando do EXO PowerShell:

    Sintaxe:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemplo: o comando a seguir irá restaurar o Subfolder1 e colocá-lo em \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Consulte [restaurar uma pasta pública excluída](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obter mais detalhes.

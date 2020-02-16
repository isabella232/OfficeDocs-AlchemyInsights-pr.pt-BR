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
# <a name="restore-a-deleted-public-folder"></a>Restaurar uma pasta pública excluída

**Para restaurar itens excluídos de uma pasta pública**:

- Confira [não é possível recuperar itens excluídos de uma pasta pública que não seja de email no Outlook 2016](https://aka.ms/pfrec).
 
**Para restaurar uma pasta pública excluída (de qualquer tipo)**: 

- Use o seguinte comando do EXO PowerShell:

    Sintaxe:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity-Path \<caminho onde a pasta será restaurada>

    Exemplo: o comando a seguir irá restaurar o Subfolder1 e colocá-lo em \Parent1:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-EQ "Subfolder1"}; Set-PublicFolder $pf. Identity-Path \Parent1

Consulte [restaurar uma pasta pública excluída](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obter mais detalhes.

---
title: A migração da pasta pública falha em 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903508"
---
# <a name="public-folder-migration-fails-at-95"></a>A migração da pasta pública falha em 95%

Para migrações de pasta pública falhando em 95%, com o erro FailedToMailEnablePublicFoldersException:

1. Baixar e executar o script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) no servidor local do Exchange.

2. Executar as ações corretivas sugeridas pelo script.

3. Executar o Sync-MailPublicFolders (para Exchange 2010) ou o Sync-ModernMailPublicFolders (para o Exchange 2013 e posteriores).

4. Retomar a migração da pasta pública.

---
title: A migração da pasta pública falha em 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: e92a983a74ac0b97a613723dacb356ebff68f6cdba2d78ca63085a818d12e739
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923299"
---
# <a name="public-folder-migration-fails-at-95"></a>A migração da pasta pública falha em 95%

Você pode ter iniciado a conclusão de um conjunto de migração, e o status do conjunto de migração continua exibindo **Sincronizado** por um tempo muito longo. Esse é comportamento esperado.

É comum que o status de um conjunto de migração permaneça em **Sincronizado** por algumas horas antes de mudar para **Completar**. Para migrações envolvendo um grande número de caixas de correio alvo, é normal ver que o status permaneça no estado de sincronização por mais de 24 horas, desde que nenhum dos pedidos de migração de pastas públicas subjacentes tenha falhado ou tenha sido colocado em quarentena. Aguarde de 24 a 48 horas para que o conjunto de migração conclua as tarefas.

Para migrações de pasta pública falhando em 95%, com o erro FailedToMailEnablePublicFoldersException:

1. Baixar e executar o script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) no servidor local do Exchange.

2. Executar as ações corretivas sugeridas pelo script.

3. Executar o Sync-MailPublicFolders (para Exchange 2010) ou o Sync-ModernMailPublicFolders (para o Exchange 2013 e posteriores).

4. Retomar a migração da pasta pública.

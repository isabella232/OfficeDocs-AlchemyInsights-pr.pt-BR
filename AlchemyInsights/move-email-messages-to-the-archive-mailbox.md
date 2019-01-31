---
title: Mover mensagens de email para a caixa de correio de arquivo morto
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660362"
---
Tendo problemas para itens na caixa de correio de arquivo morto de arquivamento. Verifique se que você executou as etapas a seguir:
  
1. Confirme que uma **caixa de correio de arquivar** tiver sido habilitado. Caso contrário, use as etapas [neste](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) artigo para habilitar a caixa de correio de arquivo morto. 
    
2. No Centro de administração do Exchange, selecione **Marcas de retenção** em **Gerenciamento de conformidade**, crie uma **marca de retenção** com a ação **Mover para arquivo morto** contendo a **Idade de retenção**de desejada.
    
3. No Centro de administração do Exchange, selecione **As políticas de retenção**, criar uma **Política de retenção** e adicionar sua marca de retenção **Mover para arquivo morto** a essa política. 
    
4. [Atribuir a política de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) a caixa de correio do usuário específico. A mesma política será aplicada a **principal** e a caixa de correio de **arquivo morto** . 
    
Caixa de correio do usuário agora deve ter uma política de arquivamento para mover itens para a caixa de correio de arquivo morto. Talvez seja necessário forçar o gerenciados pasta Assistant (MFA) para executar e aplicar as novas configurações de caixa de correio do usuário. Execute o seguinte comando enquanto [conectado ao PowerShell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de pasta gerenciada para uma caixa de correio específica: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Deseja obter mais informações sobre como configurar uma política de arquivamento, consulte [Configurar uma política de arquivamento e exclusão de caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  


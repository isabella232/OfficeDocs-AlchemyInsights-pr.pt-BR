---
title: As políticas de retenção no centro de administração do Exchange não estão funcionando
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371286"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de retenção no centro de administração do Exchange

 **Problema:** As políticas de retenção recém-criadas ou atualizadas no centro de administração do Exchange não estão aplicando caixas de correio ou itens não são movidos para a caixa de correio de arquivo morto ou excluídos. 
  
 **Causas raiz:**
  
- Talvez o **Assistente de pasta gerenciada** não tenha processado a caixa de correio do usuário. O assistente de pasta gerenciada tenta processar cada caixa de correio em sua organização baseada em nuvem uma vez a cada sete dias. Se você alterar uma marca de retenção ou aplicar uma política de retenção diferente para uma caixa de correio, poderá aguardar até que a pasta gerenciada auxiliar processe a caixa de correio ou você pode executar o cmdlet Start-ManagedFolderAssistant para iniciar o assistente de pasta gerenciada para processar um determinado nas. A execução deste cmdlet é útil para testar ou solucionar problemas de uma política de retenção ou configurações de marca de retenção. Para obter mais informações, visite [executar o assistente de pasta gerenciada](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solução:** Execute o seguinte comando para iniciar o assistente de pasta gerenciada para uma caixa de correio específica: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Isso também pode ocorrer se o **RetentionHold** tiver sido **habilitado** na caixa de correio. Se a caixa de correio tiver sido colocada em um RetentionHold, a política de retenção na caixa de correio não será processada durante esse tempo. Para mais informações sobre a configuração RetentionHold, consulte: [caixa de correio em retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solução**
    
  - Verifique o status da configuração RetentionHold na caixa de correio específica no [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Execute o seguinte comando para **desabilitar** o RetentionHold em uma caixa de correio específica: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Agora, execute novamente o assistente de pasta gerenciada:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Observação:** Se uma caixa de correio for menor do que 10 MB, o assistente de pasta gerenciada não processará automaticamente a caixa de correio. 
  


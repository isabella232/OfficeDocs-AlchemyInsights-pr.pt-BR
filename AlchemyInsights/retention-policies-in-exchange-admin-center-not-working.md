---
title: Políticas de retenção no Centro de administração do Exchange não funcionando
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274260"
---
 **Problema:** Recém-criadas ou políticas de retenção atualizado no Centro de administração do Exchange não estiver aplicando a caixas de correio ou itens não são movidas para a caixa de correio de arquivo morto ou excluídos. 
  
 **Causas raiz:**
  
- Isso pode ocorrer porque o **Assistente de pasta gerenciada** não processado caixa de correio do usuário. Assistente de pasta gerenciada tentará processar cada caixa de correio em sua organização baseada na nuvem uma vez a cada sete dias. Se você alterar uma marca de retenção ou aplica uma política de retenção diferente para uma caixa de correio, você pode aguardar até que o Assist de pasta gerenciada processa a caixa de correio ou é possível executar o cmdlet Start-ManagedFolderAssistant para iniciar o Assistente de pasta gerenciada para processar uma versão específica caixa de correio. A execução deste cmdlet é útil para testes ou solução de problemas de uma política de retenção ou as configurações de marca de retenção. Para obter mais informações, visite a [executar o Assistente de pasta gerenciada](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solução:** Execute o seguinte comando para iniciar o Assistente de pasta gerenciada para uma caixa de correio específica: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Isso também pode ocorrer se **RetentionHold** tiver sido **habilitado** na caixa de correio. Se a caixa de correio foi colocada em um RetentionHold, a política de retenção na caixa de correio não será processada durante esse horário. Para mais informações sobre a configuração e consulte RetentionHold: [Caixa de correio de retenção](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solução:**
    
  - Verificar o status da configuração de RetentionHold na caixa de correio específica no [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Execute o seguinte comando para **Desabilitar** RetentionHold em uma caixa de correio específica: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Agora, execute novamente a Assistente de pasta gerenciada:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Observação:** Se uma caixa de correio for menor do que 10 MB, Assistente de pasta gerenciada não processe automaticamente a caixa de correio. 
  


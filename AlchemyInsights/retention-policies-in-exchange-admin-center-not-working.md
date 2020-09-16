---
title: As políticas de retenção no centro de administração do Exchange não estão funcionando
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740498"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de retenção no centro de administração do Exchange

Se você quiser executar verificações automatizadas para as configurações mencionadas abaixo, selecione o botão voltar <: na parte superior desta página e insira o endereço de email do usuário que tem problemas com as políticas de retenção.

 **Problema:** As políticas de retenção recém-criadas ou atualizadas no centro de administração do Exchange não estão aplicando caixas de correio ou itens não são movidos para a caixa de correio de arquivo morto ou excluídos. 
  
 **Causas raiz:**
  
- Talvez o **Assistente de pasta gerenciada** não tenha processado a caixa de correio do usuário. O assistente de pasta gerenciada tenta processar cada caixa de correio em sua organização baseada em nuvem uma vez a cada sete dias. Se você alterar uma marca de retenção ou aplicar uma política de retenção diferente para uma caixa de correio, poderá aguardar até que a pasta gerenciada auxiliar processe a caixa de correio ou você pode executar o cmdlet Start-ManagedFolderAssistant para iniciar o assistente de pasta gerenciada para processar uma caixa de correio específica. A execução deste cmdlet é útil para testar ou solucionar problemas de uma política de retenção ou configurações de marca de retenção. Para obter mais informações, visite [executar o assistente de pasta gerenciada](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
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
 
Para obter mais informações sobre as políticas de retenção no centro de administração do Exchange, consulte:
- [Marcas e políticas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Aplicar uma política de retenção a caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adicionar ou remover marcas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Como identificar o tipo de retenção de uma caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)

---
title: Políticas de retenção no Centro de administração do Exchange não funcionando
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934980"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="cdecb-102">Políticas de retenção no Centro de administração do Exchange</span><span class="sxs-lookup"><span data-stu-id="cdecb-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="cdecb-103">**Problema:** Recém-criadas ou políticas de retenção atualizado no Centro de administração do Exchange não estiver aplicando a caixas de correio ou itens não são movidas para a caixa de correio de arquivo morto ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="cdecb-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="cdecb-104">**Causas raiz:**</span><span class="sxs-lookup"><span data-stu-id="cdecb-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="cdecb-p101">Isso pode ocorrer porque o **Assistente de pasta gerenciada** não processado caixa de correio do usuário. Assistente de pasta gerenciada tentará processar cada caixa de correio em sua organização baseada na nuvem uma vez a cada sete dias. Se você alterar uma marca de retenção ou aplica uma política de retenção diferente para uma caixa de correio, você pode aguardar até que o Assist de pasta gerenciada processa a caixa de correio ou é possível executar o cmdlet Start-ManagedFolderAssistant para iniciar o Assistente de pasta gerenciada para processar uma versão específica caixa de correio. A execução deste cmdlet é útil para testes ou solução de problemas de uma política de retenção ou as configurações de marca de retenção. Para obter mais informações, visite a [executar o Assistente de pasta gerenciada](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="cdecb-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="cdecb-110">**Solução:** Execute o seguinte comando para iniciar o Assistente de pasta gerenciada para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="cdecb-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="cdecb-p102">Isso também pode ocorrer se **RetentionHold** tiver sido **habilitado** na caixa de correio. Se a caixa de correio foi colocada em um RetentionHold, a política de retenção na caixa de correio não será processada durante esse horário. Para mais informações sobre a configuração e consulte RetentionHold: [Caixa de correio de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="cdecb-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="cdecb-114">**Solução:**</span><span class="sxs-lookup"><span data-stu-id="cdecb-114">**Solution:**</span></span>
    
  - <span data-ttu-id="cdecb-115">Verificar o status da configuração de RetentionHold na caixa de correio específica no [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="cdecb-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="cdecb-116">Execute o seguinte comando para **Desabilitar** RetentionHold em uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="cdecb-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="cdecb-117">Agora, execute novamente a Assistente de pasta gerenciada:</span><span class="sxs-lookup"><span data-stu-id="cdecb-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="cdecb-118">**Observação:** Se uma caixa de correio for menor do que 10 MB, Assistente de pasta gerenciada não processe automaticamente a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cdecb-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  


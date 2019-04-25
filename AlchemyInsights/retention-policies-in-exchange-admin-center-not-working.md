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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="12ed7-102">Políticas de retenção no centro de administração do Exchange</span><span class="sxs-lookup"><span data-stu-id="12ed7-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="12ed7-103">**Problema:** As políticas de retenção recém-criadas ou atualizadas no centro de administração do Exchange não estão aplicando caixas de correio ou itens não são movidos para a caixa de correio de arquivo morto ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="12ed7-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="12ed7-104">**Causas raiz:**</span><span class="sxs-lookup"><span data-stu-id="12ed7-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="12ed7-105">Talvez o **Assistente de pasta gerenciada** não tenha processado a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="12ed7-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="12ed7-106">O assistente de pasta gerenciada tenta processar cada caixa de correio em sua organização baseada em nuvem uma vez a cada sete dias.</span><span class="sxs-lookup"><span data-stu-id="12ed7-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="12ed7-107">Se você alterar uma marca de retenção ou aplicar uma política de retenção diferente para uma caixa de correio, poderá aguardar até que a pasta gerenciada auxiliar processe a caixa de correio ou você pode executar o cmdlet Start-ManagedFolderAssistant para iniciar o assistente de pasta gerenciada para processar um determinado nas.</span><span class="sxs-lookup"><span data-stu-id="12ed7-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="12ed7-108">A execução deste cmdlet é útil para testar ou solucionar problemas de uma política de retenção ou configurações de marca de retenção.</span><span class="sxs-lookup"><span data-stu-id="12ed7-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="12ed7-109">Para obter mais informações, visite [executar o assistente de pasta gerenciada](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="12ed7-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="12ed7-110">**Solução:** Execute o seguinte comando para iniciar o assistente de pasta gerenciada para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="12ed7-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="12ed7-111">Isso também pode ocorrer se o **RetentionHold** tiver sido **habilitado** na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12ed7-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="12ed7-112">Se a caixa de correio tiver sido colocada em um RetentionHold, a política de retenção na caixa de correio não será processada durante esse tempo.</span><span class="sxs-lookup"><span data-stu-id="12ed7-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="12ed7-113">Para mais informações sobre a configuração RetentionHold, consulte: [caixa de correio em retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="12ed7-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="12ed7-114">**Solução**</span><span class="sxs-lookup"><span data-stu-id="12ed7-114">**Solution:**</span></span>
    
  - <span data-ttu-id="12ed7-115">Verifique o status da configuração RetentionHold na caixa de correio específica no [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="12ed7-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="12ed7-116">Execute o seguinte comando para **desabilitar** o RetentionHold em uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="12ed7-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="12ed7-117">Agora, execute novamente o assistente de pasta gerenciada:</span><span class="sxs-lookup"><span data-stu-id="12ed7-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="12ed7-118">**Observação:** Se uma caixa de correio for menor do que 10 MB, o assistente de pasta gerenciada não processará automaticamente a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12ed7-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  


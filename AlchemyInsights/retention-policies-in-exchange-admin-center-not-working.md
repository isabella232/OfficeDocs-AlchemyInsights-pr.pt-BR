---
title: As políticas de retenção no centro de administração do Exchange não estão funcionando
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522795"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="7ef31-102">Políticas de retenção no centro de administração do Exchange</span><span class="sxs-lookup"><span data-stu-id="7ef31-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="7ef31-103">Se você quiser executar verificações automatizadas para as configurações mencionadas abaixo, selecione o botão voltar <: na parte superior desta página e insira o endereço de email do usuário que tem problemas com as políticas de retenção.</span><span class="sxs-lookup"><span data-stu-id="7ef31-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="7ef31-104">**Problema:** As políticas de retenção recém-criadas ou atualizadas no centro de administração do Exchange não estão aplicando caixas de correio ou itens não são movidos para a caixa de correio de arquivo morto ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="7ef31-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="7ef31-105">**Causas raiz:**</span><span class="sxs-lookup"><span data-stu-id="7ef31-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="7ef31-106">Talvez o **Assistente de pasta gerenciada** não tenha processado a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="7ef31-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="7ef31-107">O assistente de pasta gerenciada tenta processar cada caixa de correio em sua organização baseada em nuvem uma vez a cada sete dias.</span><span class="sxs-lookup"><span data-stu-id="7ef31-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="7ef31-108">Se você alterar uma marca de retenção ou aplicar uma política de retenção diferente para uma caixa de correio, poderá aguardar até que a pasta gerenciada auxiliar processe a caixa de correio ou você pode executar o cmdlet Start-ManagedFolderAssistant para iniciar o assistente de pasta gerenciada para processar uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="7ef31-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="7ef31-109">A execução deste cmdlet é útil para testar ou solucionar problemas de uma política de retenção ou configurações de marca de retenção.</span><span class="sxs-lookup"><span data-stu-id="7ef31-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="7ef31-110">Para obter mais informações, visite [executar o assistente de pasta gerenciada](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="7ef31-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="7ef31-111">**Solução:** Execute o seguinte comando para iniciar o assistente de pasta gerenciada para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="7ef31-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="7ef31-112">Isso também pode ocorrer se o **RetentionHold** tiver sido **habilitado** na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ef31-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="7ef31-113">Se a caixa de correio tiver sido colocada em um RetentionHold, a política de retenção na caixa de correio não será processada durante esse tempo.</span><span class="sxs-lookup"><span data-stu-id="7ef31-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="7ef31-114">Para mais informações sobre a configuração RetentionHold, consulte: [caixa de correio em retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="7ef31-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="7ef31-115">**Solução**</span><span class="sxs-lookup"><span data-stu-id="7ef31-115">**Solution:**</span></span>
    
  - <span data-ttu-id="7ef31-116">Verifique o status da configuração RetentionHold na caixa de correio específica no [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="7ef31-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="7ef31-117">Execute o seguinte comando para **desabilitar** o RetentionHold em uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="7ef31-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="7ef31-118">Agora, execute novamente o assistente de pasta gerenciada:</span><span class="sxs-lookup"><span data-stu-id="7ef31-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="7ef31-119">**Observação:** Se uma caixa de correio for menor do que 10 MB, o assistente de pasta gerenciada não processará automaticamente a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ef31-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="7ef31-120">Para obter mais informações sobre as políticas de retenção no centro de administração do Exchange, consulte:</span><span class="sxs-lookup"><span data-stu-id="7ef31-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="7ef31-121">Marcas e políticas de retenção</span><span class="sxs-lookup"><span data-stu-id="7ef31-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="7ef31-122">Aplicar uma política de retenção a caixas de correio</span><span class="sxs-lookup"><span data-stu-id="7ef31-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="7ef31-123">Adicionar ou remover marcas de retenção</span><span class="sxs-lookup"><span data-stu-id="7ef31-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="7ef31-124">Como identificar o tipo de retenção de uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7ef31-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)

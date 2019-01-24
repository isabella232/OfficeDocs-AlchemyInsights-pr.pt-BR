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
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457115"
---
<span data-ttu-id="08916-p101">Tendo problemas para itens na caixa de correio de arquivo morto de arquivamento. Verifique se que você executou as etapas a seguir:</span><span class="sxs-lookup"><span data-stu-id="08916-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="08916-p102">Confirme que uma **caixa de correio de arquivar** tiver sido habilitado. Caso contrário, use as etapas [neste](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) artigo para habilitar a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="08916-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="08916-106">No Centro de administração do Exchange, selecione **Marcas de retenção** em **Gerenciamento de conformidade**, crie uma **marca de retenção** com a ação **Mover para arquivo morto** contendo a **Idade de retenção**de desejada.</span><span class="sxs-lookup"><span data-stu-id="08916-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="08916-107">No Centro de administração do Exchange, selecione **As políticas de retenção**, criar uma **Política de retenção** e adicionar sua marca de retenção **Mover para arquivo morto** a essa política.</span><span class="sxs-lookup"><span data-stu-id="08916-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="08916-p103">[Atribuir a política de retenção](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) a caixa de correio do usuário específico. A mesma política será aplicada a **principal** e a caixa de correio de **arquivo morto** .</span><span class="sxs-lookup"><span data-stu-id="08916-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="08916-p104">Caixa de correio do usuário agora deve ter uma política de arquivamento para mover itens para a caixa de correio de arquivo morto. Talvez seja necessário forçar o gerenciados pasta Assistant (MFA) para executar e aplicar as novas configurações de caixa de correio do usuário. Execute o seguinte comando enquanto [conectado ao PowerShell EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o Assistente de pasta gerenciada para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="08916-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="08916-113">Deseja obter mais informações sobre como configurar uma política de arquivamento, consulte [Configurar uma política de arquivamento e exclusão de caixas de correio](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="08916-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  


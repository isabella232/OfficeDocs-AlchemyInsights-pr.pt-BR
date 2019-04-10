---
title: Mover mensagens de email para a caixa de correio de arquivo morto
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747191"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="a39c9-102">Mover email para a caixa de correio de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="a39c9-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="a39c9-103">Confirmar se uma **caixa de correio de arquivo morto** foi habilitada.</span><span class="sxs-lookup"><span data-stu-id="a39c9-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="a39c9-104">Caso contrário, use as etapas neste [artigo](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) para habilitar a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="a39c9-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="a39c9-105">Para arquivar mensagens automaticamente na caixa de correio de arquivo morto, uma marca de retenção com a ação **mover para arquivo morto** deve ser definida como **aplicada automaticamente à marca de caixa de correio inteira (padrão)**.</span><span class="sxs-lookup"><span data-stu-id="a39c9-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="a39c9-106">Use as etapas aqui para criar a marca de formatação: [arquivo morto padrão](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="a39c9-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="a39c9-107">Em seguida, adicione a marca **Archive** à sua política de retenção.</span><span class="sxs-lookup"><span data-stu-id="a39c9-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="a39c9-108">No centro de administração do Exchange, escolha **políticas de retenção** > adicionar a **marca mover para arquivo morto** à política > **salvar**.</span><span class="sxs-lookup"><span data-stu-id="a39c9-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="a39c9-109">Agora, [atribua a política de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) à caixa de correio do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="a39c9-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="a39c9-110">A mesma política será aplicada à caixa de correio **principal** e de **arquivo morto** .</span><span class="sxs-lookup"><span data-stu-id="a39c9-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="a39c9-111">Pode ser necessário forçar o assistente de pasta gerenciada (MFA) a ser executado e aplicar as novas configurações à caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a39c9-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="a39c9-112">Execute o seguinte comando enquanto [estiver conectado ao EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar o assistente de pasta gerenciada para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="a39c9-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="a39c9-113">Para obter mais informações sobre como configurar uma política de arquivo morto, consulte [Configurar uma política de arquivo morto e exclusão para caixas de correio](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="a39c9-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  


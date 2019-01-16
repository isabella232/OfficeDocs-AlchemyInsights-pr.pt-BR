---
title: Pasta de RecoverableItems 1336 está cheio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274621"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="2fceb-102">A pasta itens recuperáveis está cheio</span><span class="sxs-lookup"><span data-stu-id="2fceb-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="2fceb-p101">Para caixas de correio Exchange Online no Office 365, o limite de armazenamento padrão para a pasta itens recuperáveis é 30 GB. O limite de armazenamento para a pasta itens recuperáveis automaticamente é aumentado para 100 GB se a caixa de correio for colocada em retenção de litígio, retenção de descoberta eletrônica ou é atribuída a uma política de retenção do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2fceb-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="2fceb-105">Quando a pasta itens recuperáveis atinge o limite de armazenamento, a funcionalidade de caixa de correio é afetada das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="2fceb-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="2fceb-106">O usuário não pode excluir itens da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2fceb-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="2fceb-107">O Assistente de Pasta Gerenciada não pode excluir itens com base na marca de retenção ou nas configurações de pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="2fceb-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="2fceb-108">Para caixas de correio que tenham a recuperação de Item único habilitada ou são colocadas em espera, o processo de proteção de página de cópia-na-gravação não pode manter versões dos itens editados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="2fceb-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="2fceb-109">Para caixas de correio que tem a caixa de correio habilitada de log de auditoria, nenhuma entrada de log de auditoria de caixa de correio pode ser salvas na subpasta auditorias na pasta itens recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="2fceb-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="2fceb-p102">Para caixas de correio que não estão em espera, os administradores podem usar o `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command no PowerShell do Exchange Online para excluir itens na pasta itens recuperáveis. Para obter mais informações, consulte os tópicos a seguir:</span><span class="sxs-lookup"><span data-stu-id="2fceb-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="2fceb-112">Procurar e excluir mensagens</span><span class="sxs-lookup"><span data-stu-id="2fceb-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="2fceb-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="2fceb-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="2fceb-p103">Para caixas de correio que estiverem em espera, os administradores precisa remover a retenção antes que eles podem itens excluídos da pasta itens recuperáveis. Para obter mais informações, consulte [Excluir itens na pasta de caixas de correio baseadas em nuvem em espera itens recuperáveis](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="2fceb-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="2fceb-p104">Para ajudar a evitar que a pasta itens recuperáveis se torne completa, os administradores podem aumentar o limite de armazenamento dos itens recuperáveis pasta para caixas de correio em espera e definir uma política de retenção de caixa de correio que move itens da pasta itens recuperáveis para o arquivo do usuário caixa de correio. Consulte [aumentar a cota de caixas de correio em retenção de itens recuperáveis](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="2fceb-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  


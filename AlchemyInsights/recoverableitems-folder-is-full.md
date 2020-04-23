---
title: 1336 a pasta RecoverableItems está cheia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720240"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="49575-102">A pasta itens recuperáveis está cheia</span><span class="sxs-lookup"><span data-stu-id="49575-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="49575-103">Para caixas de correio do Exchange Online, o limite de armazenamento padrão para a pasta itens recuperáveis é de 30 GB.</span><span class="sxs-lookup"><span data-stu-id="49575-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="49575-104">O limite de armazenamento da pasta itens recuperáveis é aumentado automaticamente para 100 GB se a caixa de correio for colocada em retenção de litígio, retenção de descoberta eletrônica ou atribuída a uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="49575-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="49575-105">Quando a pasta itens recuperáveis atinge o limite de armazenamento, a funcionalidade de caixa de correio é afetada das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="49575-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="49575-106">O usuário não pode excluir itens da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="49575-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="49575-107">O Assistente de Pasta Gerenciada não pode excluir itens com base na marca de retenção ou nas configurações de pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="49575-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="49575-108">Para caixas de correio que têm a recuperação de item único habilitada ou são colocadas em espera, o processo de proteção de página de cópia de gravação não pode manter versões de itens editadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="49575-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="49575-109">Para caixas de correio com registro em log de auditoria de caixa de correio habilitado, nenhuma entrada de log de auditoria de caixa de correio pode ser salva na subpasta auditorias da pasta itens recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="49575-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="49575-110">Para caixas de correio que não estão em retenção, os administradores `Search-Mailbox -SearchDumpsterOnly -DeleteContent` podem usar o comando no PowerShell do Exchange Online para excluir itens na pasta itens recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="49575-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="49575-111">Para mais informações, confira os seguintes tópicos:</span><span class="sxs-lookup"><span data-stu-id="49575-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="49575-112">Procurar e excluir mensagens</span><span class="sxs-lookup"><span data-stu-id="49575-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="49575-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="49575-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="49575-114">Para caixas de correio em espera, os administradores precisam remover a retenção antes de poderem excluir itens da pasta itens recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="49575-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="49575-115">Para obter mais informações, consulte [excluir itens na pasta itens recuperáveis de caixas de correio baseadas em nuvem em espera](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="49575-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="49575-116">Para ajudar a evitar que a pasta de itens recuperáveis fique cheia, os administradores podem aumentar o limite de armazenamento da pasta itens recuperáveis para caixas de correio em espera e configurar uma política de retenção de caixa de correio que move itens da pasta itens recuperáveis para a caixa de correio de arquivo morto do usuário.</span><span class="sxs-lookup"><span data-stu-id="49575-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="49575-117">Consulte [aumentar a cota de itens recuperáveis para caixas de correio em espera](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="49575-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>

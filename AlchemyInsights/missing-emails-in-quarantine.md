---
title: Ausência de emails em quarentena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542073"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="54495-102">Emails ausentes em quarentena "</span><span class="sxs-lookup"><span data-stu-id="54495-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="54495-103">Os administradores podem [Exibir, liberar ou excluir essas mensagens.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="54495-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="54495-104">Para abrir o centro de conformidade & segurança, vá para [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="54495-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="54495-105">Para abrir a página de quarentena diretamente, acesse [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="54495-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="54495-106">Você pode pesquisar pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="54495-106">You can search by the following values:</span></span>  

- <span data-ttu-id="54495-107">**ID da mensagem**: o identificador globalmente exclusivo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54495-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="54495-108">Se você selecionar uma mensagem na lista, o valor **ID da mensagem** aparecerá no painel de submenu **detalhes** exibido.</span><span class="sxs-lookup"><span data-stu-id="54495-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="54495-109">Os administradores podem usar [Rastreamento da mensagem](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para localizar mensagens e seus valores da ID da mensagem correspondentes.</span><span class="sxs-lookup"><span data-stu-id="54495-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="54495-110">**Endereço de e-mail do remetente**: o endereço de e-mail de um único remetente.</span><span class="sxs-lookup"><span data-stu-id="54495-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="54495-111">**Endereço de e-mail do destinatário**: o endereço de e-mail de um único destinatário.</span><span class="sxs-lookup"><span data-stu-id="54495-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="54495-112">**Assunto**: use todo o assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54495-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="54495-113">A pesquisa não diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="54495-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="54495-114">Depois de inserir os critérios de pesquisa, clique em ![ Atualizar botão ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atualizar** para filtrar os resultados.  </span><span class="sxs-lookup"><span data-stu-id="54495-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="54495-115">Os cmdlets que você usa para exibir e gerenciar mensagens e arquivos em quarentena são:</span><span class="sxs-lookup"><span data-stu-id="54495-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="54495-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="54495-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="54495-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="54495-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="54495-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="54495-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="54495-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Observe que este cmdlet é somente para mensagens, e não para arquivos de malware de ATP para SharePoint Online, onedrive for Business ou Teams.</span><span class="sxs-lookup"><span data-stu-id="54495-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="54495-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="54495-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
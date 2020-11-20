---
title: Cancelar ou substituir uma mensagem de email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353494"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="b11d4-102">Cancelar ou substituir uma mensagem de email no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b11d4-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="b11d4-103">Você **só pode recuperar mensagens que são enviadas para pessoas em sua organização**.</span><span class="sxs-lookup"><span data-stu-id="b11d4-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b11d4-104">Por exemplo, se a mensagem foi enviada para um endereço do Gmail, você não poderá recuperá-la.</span><span class="sxs-lookup"><span data-stu-id="b11d4-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="b11d4-105">Você pode **apenas recuperar mensagens enviadas do Outlook para o PC**.</span><span class="sxs-lookup"><span data-stu-id="b11d4-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="b11d4-106">Se um usuário enviar uma mensagem usando o Outlook para Mac ou o Outlook na Web, você não poderá recuperá-la.</span><span class="sxs-lookup"><span data-stu-id="b11d4-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="b11d4-107">Como administrador de locatários, você pode **recuperar mensagens em nome dos usuários usando o PowerShell** (para obter mais informações, consulte: [Pesquisar e excluir mensagens de email](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="b11d4-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="b11d4-108">Não é possível recuperar mensagens do centro de administração.</span><span class="sxs-lookup"><span data-stu-id="b11d4-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="b11d4-109">Role para baixo até "procurar e excluir mensagens de email em sua organização" para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="b11d4-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="b11d4-110">**Cancelar ou substituir uma mensagem de email enviada**</span><span class="sxs-lookup"><span data-stu-id="b11d4-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="b11d4-111">No painel de pastas à esquerda da janela do Outlook, escolha a pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="b11d4-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="b11d4-112">Abra a mensagem que você deseja cancelar.</span><span class="sxs-lookup"><span data-stu-id="b11d4-112">Open the message that you want to recall.</span></span> <span data-ttu-id="b11d4-113">Você deve clicar duas vezes para abrir a mensagem.</span><span class="sxs-lookup"><span data-stu-id="b11d4-113">You must double-click to open the message.</span></span> <span data-ttu-id="b11d4-114">Selecionar a mensagem para que ela apareça no painel de leitura não permite que você relembre a mensagem.</span><span class="sxs-lookup"><span data-stu-id="b11d4-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="b11d4-115">Na guia mensagem, selecione **ações**  >  **cancelar esta mensagem**.</span><span class="sxs-lookup"><span data-stu-id="b11d4-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="b11d4-116">Escolha **Excluir cópias não lidas desta mensagem** ou **Excluir cópias não lidas e substituir por uma nova mensagem** e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="b11d4-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="b11d4-117">Se você estiver enviando uma mensagem de substituição, redija a mensagem e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="b11d4-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="b11d4-118">O sucesso ou a falha de uma recuperação de mensagem depende das configurações dos destinatários no Outlook.</span><span class="sxs-lookup"><span data-stu-id="b11d4-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="b11d4-119">Para obter mais informações, incluindo como verificar o cancelamento, confira [cancelar ou substituir uma mensagem de email enviada](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="b11d4-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b11d4-120">**_Para pesquisar e excluir mensagens de email em sua organização_**, é mais fácil se você for um administrador global. Se você não for um administrador global, sua conta deverá ser adicionada ao grupo de funções Gerenciador de descoberta eletrônica ou à função de gerenciamento de pesquisa de conformidade.</span><span class="sxs-lookup"><span data-stu-id="b11d4-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="b11d4-121">Para excluir mensagens, você precisará ingressar no grupo de função gerenciamento da organização ou na função gerenciamento de pesquisa e limpeza.</span><span class="sxs-lookup"><span data-stu-id="b11d4-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b11d4-122">As permissões para essas funções são atribuídas no [centro de conformidade de & de segurança](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="b11d4-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="b11d4-123">[Criar uma pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/content-search) para localizar a mensagem a ser excluída.</span><span class="sxs-lookup"><span data-stu-id="b11d4-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="b11d4-124">[Conectar-se ao Windows PowerShell do Centro de Conformidade e Segurança](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b11d4-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="b11d4-125">Se você estiver usando a MFA (autenticação multifator), confira [conectar-se ao PowerShell do centro de conformidade do Microsoft 365 Security & usando a autenticação multifator](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b11d4-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>

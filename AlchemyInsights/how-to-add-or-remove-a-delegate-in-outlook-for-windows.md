---
title: Como adicionar ou remover um representante no Outlook para Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571769"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="07277-102">Como adicionar ou remover um representante no Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="07277-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="07277-103">Para adicionar um representante no Outlook para Windows:</span><span class="sxs-lookup"><span data-stu-id="07277-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="07277-104">Clique na guia **arquivo** seguida por **configurações de conta** e escolha acesso de **Representante**.</span><span class="sxs-lookup"><span data-stu-id="07277-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="07277-105">Clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="07277-105">Click on **Add**.</span></span> <span data-ttu-id="07277-106">Se **Add** não aparecer, uma conexão ativa pode não existir entre o Outlook e o Exchange.</span><span class="sxs-lookup"><span data-stu-id="07277-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="07277-107">A barra de status do Outlook exibe o status da conexão.</span><span class="sxs-lookup"><span data-stu-id="07277-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="07277-108">Digite o nome da pessoa que você deseja designar como seu representante ou pesquise e escolha o nome na lista de resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="07277-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="07277-109">O representante deve ser uma pessoa na GAL (lista de endereços global) do Exchange da sua organização.</span><span class="sxs-lookup"><span data-stu-id="07277-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="07277-110">Clique em **Adicionar** seguido por **OK**.</span><span class="sxs-lookup"><span data-stu-id="07277-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="07277-111">Na caixa de diálogo **permissões de representante** , aceite as configurações de permissão padrão ou selecione níveis de acesso personalizados para pastas do Exchange.</span><span class="sxs-lookup"><span data-stu-id="07277-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="07277-112">Se um representante precisar de permissão para trabalhar apenas com solicitações de reunião e respostas, as configurações de permissão padrão, como **Representante, receberá cópias de mensagens relacionadas à reunião enviadas para mim** são suficientes.</span><span class="sxs-lookup"><span data-stu-id="07277-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="07277-113">Você pode deixar a configuração de permissão de **caixa de entrada** como **nenhum**.</span><span class="sxs-lookup"><span data-stu-id="07277-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="07277-114">As solicitações e respostas de reunião vão diretamente para a caixa de entrada do representante.</span><span class="sxs-lookup"><span data-stu-id="07277-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="07277-115">Por padrão, o representante tem a permissão **Editor (pode ler, criar e modificar itens)** na pasta **calendário** .</span><span class="sxs-lookup"><span data-stu-id="07277-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="07277-116">Quando o representante responde a uma reunião em seu nome, ele é automaticamente adicionado à pasta **calendário** .</span><span class="sxs-lookup"><span data-stu-id="07277-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="07277-117">Para enviar uma mensagem para notificar o representante das permissões alteradas, marque a caixa de seleção **Enviar automaticamente uma mensagem para o representante Resumindo estas permissões** .</span><span class="sxs-lookup"><span data-stu-id="07277-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="07277-118">Se desejar, marque a caixa de seleção **Representante pode ver meus itens particulares** .</span><span class="sxs-lookup"><span data-stu-id="07277-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="07277-119">Essa configuração afeta todas as pastas do Exchange.</span><span class="sxs-lookup"><span data-stu-id="07277-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="07277-120">Isso inclui todos os emails, contatos, calendário, tarefas, anotações e pastas de diário.</span><span class="sxs-lookup"><span data-stu-id="07277-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="07277-121">Não há como conceder acesso a itens privados em apenas pastas especificadas.</span><span class="sxs-lookup"><span data-stu-id="07277-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="07277-122">Escolha **OK**.</span><span class="sxs-lookup"><span data-stu-id="07277-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="07277-123">As mensagens enviadas com as permissões Enviar em nome de incluem o representante **de**.</span><span class="sxs-lookup"><span data-stu-id="07277-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="07277-124">Quando uma mensagem é enviada com permissões Enviar como, apenas seu nome é exibido.</span><span class="sxs-lookup"><span data-stu-id="07277-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="07277-125">Depois que você adicionar alguém como representante, poderá adicionar sua caixa de correio do Exchange ao seu perfil do Outlook.</span><span class="sxs-lookup"><span data-stu-id="07277-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="07277-126">Para obter instruções, consulte [gerenciar itens de email e calendário de outra pessoa](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="07277-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="07277-127">Para remover um representante no Outlook para Windows:</span><span class="sxs-lookup"><span data-stu-id="07277-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="07277-128">Clique na guia **arquivo** .</span><span class="sxs-lookup"><span data-stu-id="07277-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="07277-129">Clique em **configurações de conta** seguidas por **acesso de representante**.</span><span class="sxs-lookup"><span data-stu-id="07277-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="07277-130">Escolha o nome do representante para o qual você deseja alterar as permissões e clique em **remover** seguido por **OK**.</span><span class="sxs-lookup"><span data-stu-id="07277-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>

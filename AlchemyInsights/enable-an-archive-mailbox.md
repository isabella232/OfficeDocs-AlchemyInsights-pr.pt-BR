---
title: Habilitar uma caixa de correio de arquivo morto
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811693"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="866f4-102">Habilitar uma caixa de correio de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="866f4-102">Enable an archive mailbox</span></span>

<span data-ttu-id="866f4-103">Se quiser que possamos executar verificações automatizadas para garantir que uma caixa de correio de arquivo morto possa ser configurada, selecione o botão voltar <-no início dessa página e insira o endereço de email da conta.</span><span class="sxs-lookup"><span data-stu-id="866f4-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="866f4-104">As caixas de correio de arquivo morto no Microsoft 365 (também chamadas de *arquivos online* ou *arquivos mortos locais*) fornecem aos usuários um armazenamento de email adicional.</span><span class="sxs-lookup"><span data-stu-id="866f4-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="866f4-105">Os usuários podem mover ou copiar itens para a caixa de correio de arquivo morto, e os administradores podem criar uma política de arquivamento que move automaticamente itens para caixas de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="866f4-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="866f4-106">Confira aqui como criar uma caixa de correio de arquivo morto:</span><span class="sxs-lookup"><span data-stu-id="866f4-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="866f4-107">Acesse [https://protection.office.com](https://protection.office.com).</span><span class="sxs-lookup"><span data-stu-id="866f4-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="866f4-108">Entre no Microsoft 365 usando sua conta de administrador.</span><span class="sxs-lookup"><span data-stu-id="866f4-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="866f4-109">No painel esquerdo do centro de conformidade de segurança &amp; , selecione **Information governance** \> **arquivamento**de governança de informações.</span><span class="sxs-lookup"><span data-stu-id="866f4-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="866f4-110">Selecione o usuário cuja caixa de correio de arquivo morto você deseja habilitar.</span><span class="sxs-lookup"><span data-stu-id="866f4-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="866f4-111">No painel de detalhes à direita, clique em **habilitar** e, em seguida, clique em **Sim** na mensagem de aviso para habilitar a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="866f4-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="866f4-112">Você também pode habilitar as caixas de correio de arquivo morto em massa, selecionando vários usuários (usando as teclas **Shift** ou **Ctrl** ) e clicando em **habilitar** no painel de detalhes.</span><span class="sxs-lookup"><span data-stu-id="866f4-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="866f4-113">Caixas de correio compartilhadas</span><span class="sxs-lookup"><span data-stu-id="866f4-113">Shared mailboxes</span></span>

<span data-ttu-id="866f4-114">Para habilitar o arquivo morto para uma caixa de correio compartilhada, uma licença do Exchange Online Plan 2 ou uma licença do plano 1 do Exchange Online com uma licença de arquivamento do Exchange Online é necessária.</span><span class="sxs-lookup"><span data-stu-id="866f4-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="866f4-115">Para habilitar o arquivo morto para uma caixa de correio compartilhada:</span><span class="sxs-lookup"><span data-stu-id="866f4-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="866f4-116">Vá para o [centro de administração do Exchange](https://outlook.office365.com/ecp) e entre usando sua conta de administrador.</span><span class="sxs-lookup"><span data-stu-id="866f4-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="866f4-117">Vá para **destinatários**  >  **compartilhados**.</span><span class="sxs-lookup"><span data-stu-id="866f4-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="866f4-118">Selecione a caixa de correio compartilhada.</span><span class="sxs-lookup"><span data-stu-id="866f4-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="866f4-119">No painel de detalhes à direita, em **arquivo in-loco**, clique em **habilitar**e, em seguida, clique em **Sim** para habilitar a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="866f4-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="866f4-120">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="866f4-120">For more information, see:</span></span>
  
- [<span data-ttu-id="866f4-121">Habilitar caixas de correio de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="866f4-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="866f4-122">Configurar uma política de arquivo morto e exclusão</span><span class="sxs-lookup"><span data-stu-id="866f4-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

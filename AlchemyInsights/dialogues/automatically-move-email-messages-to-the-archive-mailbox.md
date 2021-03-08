---
title: Mover automaticamente mensagens de email para a caixa de correio de arquivo morto
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522350"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="f8310-102">Mover automaticamente mensagens de email para a caixa de correio de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="f8310-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="f8310-103">Veja como configurar uma política para mover automaticamente o email antigo de um usuário para a caixa de correio de arquivo morto:</span><span class="sxs-lookup"><span data-stu-id="f8310-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="f8310-104">Acesse [**Security & Compliance Data**](https://go.microsoft.com/fwlink/p/?linkid=2077143)governance Archive para verificar se uma caixa de correio de arquivo morto  >    >   foi habilitada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="f8310-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="f8310-105">Se não tiver, clique em **Habilitar,** **em seguida, Sim** na caixa de aviso.</span><span class="sxs-lookup"><span data-stu-id="f8310-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="f8310-106">Vá para o [**Centro de administração do Exchange > gerenciamento de conformidade > marcas de retenção**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="f8310-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="f8310-107">Escolha o ícone + e escolha **aplicar automaticamente a caixa de correio inteira.**</span><span class="sxs-lookup"><span data-stu-id="f8310-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="f8310-108">Atribua um nome à marca de retenção e escolha **Mover para Arquivar**.</span><span class="sxs-lookup"><span data-stu-id="f8310-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="f8310-109">Para o período de retenção, insira o tempo que você deseja, como 90 dias.</span><span class="sxs-lookup"><span data-stu-id="f8310-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="f8310-110">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="f8310-110">Click **Save**.</span></span>
5. <span data-ttu-id="f8310-111">Agora crie uma política de retenção: escolha **políticas de** retenção , escolha o ícone para adicionar uma nova política.</span><span class="sxs-lookup"><span data-stu-id="f8310-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="f8310-112">Atribua um nome à política de retenção e clique e role para encontrar e adicionar a marca de retenção que você acabou de criar.</span><span class="sxs-lookup"><span data-stu-id="f8310-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="f8310-113">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="f8310-113">Click **Save**.</span></span>
7. <span data-ttu-id="f8310-114">Por fim, aplique a política de retenção à caixa de correio do usuário: ainda no Centro de administração do Exchange, vá para caixas **de** correio  >  **de destinatários.**</span><span class="sxs-lookup"><span data-stu-id="f8310-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="f8310-115">Escolha todos os usuários aos quais você deseja aplicar a política e escolha **Editar** (o ícone do lápis).</span><span class="sxs-lookup"><span data-stu-id="f8310-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="f8310-116">Na caixa de diálogo, clique em recursos **de caixa de correio**.</span><span class="sxs-lookup"><span data-stu-id="f8310-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="f8310-117">Em **Política de retenção,** aplique a política que você acabou de criar > **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="f8310-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="f8310-118">Para obter instruções para aplicar a política a todos os usuários, consulte [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="f8310-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>

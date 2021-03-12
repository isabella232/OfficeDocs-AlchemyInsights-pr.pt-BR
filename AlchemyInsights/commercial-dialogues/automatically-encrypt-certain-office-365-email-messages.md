---
title: Criptografar automaticamente determinadas mensagens de email do Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735390"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="95b8b-102">Criptografar automaticamente determinadas mensagens de email do Office 365</span><span class="sxs-lookup"><span data-stu-id="95b8b-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="95b8b-103">Você pode criptografar automaticamente mensagens que os usuários enviam para determinadas pessoas ou organizações externas.</span><span class="sxs-lookup"><span data-stu-id="95b8b-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="95b8b-104">Para fazer isso, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="95b8b-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="95b8b-105">No Centro [de administração do Exchange,](https://outlook.office365.com/ecp/)escolha **fluxo de emails > regras.**</span><span class="sxs-lookup"><span data-stu-id="95b8b-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="95b8b-106">Clique no **ícone Novo (+)** e, em seguida, clique em Aplicar a Criptografia de Mensagens do **Office 365 e proteção de** direitos às mensagens .</span><span class="sxs-lookup"><span data-stu-id="95b8b-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="95b8b-107">Em **Nome**, insira um nome para a regra, como *Criptografar mensagens enviadas para DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="95b8b-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="95b8b-108">In **Apply this rule if**, choose The recipient > is this **person**.</span><span class="sxs-lookup"><span data-stu-id="95b8b-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="95b8b-109">Na janela **Selecionar Membros,** selecione o nome da pessoa à quem você deseja aplicar a regra de criptografia e clique em **adicionar**.</span><span class="sxs-lookup"><span data-stu-id="95b8b-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="95b8b-110">Quando terminar de adicionar usuários, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="95b8b-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="95b8b-111">Ao lado do **campo Fazer o seguinte,** clique **em Selecionar um**.</span><span class="sxs-lookup"><span data-stu-id="95b8b-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="95b8b-112">No menu **suspenso do modelo RMS,** selecione **Criptografar** e clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="95b8b-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="95b8b-113">(Se você não vir essa opção, isso significa que seu plano não inclui criptografia automática.</span><span class="sxs-lookup"><span data-stu-id="95b8b-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="95b8b-114">Mas você pode adicioná-lo!)</span><span class="sxs-lookup"><span data-stu-id="95b8b-114">But you can add it!)</span></span>
9. <span data-ttu-id="95b8b-115">Escolha qualquer seleção opcional (em uma lista de seleções opcionais que você pode fazer neste ponto, muitas das quais podem ser deixadas com a configuração padrão para simplicidade).</span><span class="sxs-lookup"><span data-stu-id="95b8b-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="95b8b-116">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="95b8b-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="95b8b-117">Você sempre pode voltar e editar essa regra mais tarde.</span><span class="sxs-lookup"><span data-stu-id="95b8b-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="95b8b-118">Para obter mais informações sobre como criar regras para criptografia, consulte Definir regras de fluxo de emails para criptografar mensagens de [email no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="95b8b-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>


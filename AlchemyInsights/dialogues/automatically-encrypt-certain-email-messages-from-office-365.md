---
title: Criptografar automaticamente determinadas mensagens de email do office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509555"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="c2a45-102">Criptografar automaticamente determinadas mensagens de email do office 365</span><span class="sxs-lookup"><span data-stu-id="c2a45-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="c2a45-103">No Centro [de administração do Exchange,](https://outlook.office365.com/ecp/)escolha **fluxo de emails > regras.**</span><span class="sxs-lookup"><span data-stu-id="c2a45-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c2a45-104">Clique no **ícone Novo (+)** e, em seguida, clique em Aplicar a Criptografia de Mensagens do **Office 365 e proteção de** direitos às mensagens .</span><span class="sxs-lookup"><span data-stu-id="c2a45-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c2a45-105">Em **Nome**, insira um nome para a regra, como *Criptografar todas as mensagens*.</span><span class="sxs-lookup"><span data-stu-id="c2a45-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="c2a45-106">Em **Aplicar essa regra se**, escolha **[Aplicar a todas as mensagens]**.</span><span class="sxs-lookup"><span data-stu-id="c2a45-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="c2a45-107">Ao lado do **campo Fazer o seguinte,** clique **em Selecionar um**.</span><span class="sxs-lookup"><span data-stu-id="c2a45-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="c2a45-108">No menu **suspenso do modelo RMS,** selecione **Criptografar** e clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="c2a45-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c2a45-109">(Se você não vir essa opção, isso significa que seu plano não inclui criptografia automática.</span><span class="sxs-lookup"><span data-stu-id="c2a45-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c2a45-110">Mas você pode adicioná-lo!)</span><span class="sxs-lookup"><span data-stu-id="c2a45-110">But you can add it!)</span></span>
7. <span data-ttu-id="c2a45-111">Marque a **caixa de seleção Auditar** essa regra com nível de gravidade e selecione o nível desejado.</span><span class="sxs-lookup"><span data-stu-id="c2a45-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="c2a45-112">Se sua empresa tiver obrigações contratuais para enviar todos os emails criptografados, recomendamos definir o nível como **Alto**.</span><span class="sxs-lookup"><span data-stu-id="c2a45-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="c2a45-113">Em **Escolher um modelo para essa regra,** clique em **Impor**.</span><span class="sxs-lookup"><span data-stu-id="c2a45-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="c2a45-114">Escolha qualquer seleção opcional (em uma lista de seleções opcionais que você pode fazer neste ponto, muitas das quais podem ser deixadas com a configuração padrão para simplicidade).</span><span class="sxs-lookup"><span data-stu-id="c2a45-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c2a45-115">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="c2a45-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c2a45-116">Você sempre pode voltar e editar essa regra mais tarde.</span><span class="sxs-lookup"><span data-stu-id="c2a45-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c2a45-117">Para obter mais informações sobre como criar regras para criptografia, consulte Definir regras de fluxo de emails [para criptografar mensagens de email no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="c2a45-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>


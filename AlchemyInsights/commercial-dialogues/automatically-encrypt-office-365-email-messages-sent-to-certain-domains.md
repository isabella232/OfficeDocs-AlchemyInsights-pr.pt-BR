---
title: Criptografar automaticamente mensagens de email do Office 365 enviadas para determinados domínios
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735379"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="2c5eb-102">Criptografar automaticamente mensagens de email do Office 365 enviadas para determinados domínios</span><span class="sxs-lookup"><span data-stu-id="2c5eb-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="2c5eb-103">No Centro [de administração do Exchange,](https://outlook.office365.com/ecp/)escolha **fluxo de emails > regras.**</span><span class="sxs-lookup"><span data-stu-id="2c5eb-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="2c5eb-104">Clique no **ícone Novo (+)** e, em seguida, clique em Aplicar a Criptografia de Mensagens do **Office 365 e proteção de** direitos às mensagens .</span><span class="sxs-lookup"><span data-stu-id="2c5eb-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="2c5eb-105">Em **Nome**, insira um nome para a regra, como *Criptografar mensagens enviadas para contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="2c5eb-106">In **Apply this rule if**, choose The recipient > domain **is**.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="2c5eb-107">Insira o nome do domínio, como **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="2c5eb-108">Clique no **ícone Adicionar (+)** e clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="2c5eb-109">Ao lado do **campo Fazer o seguinte,** clique **em Selecionar um**.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="2c5eb-110">No menu **suspenso do modelo RMS,** selecione **Criptografar** e clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="2c5eb-111">(Se você não vir essa opção, isso significa que seu plano não inclui criptografia automática.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="2c5eb-112">Mas você pode adicioná-lo!)</span><span class="sxs-lookup"><span data-stu-id="2c5eb-112">But you can add it!)</span></span>
9. <span data-ttu-id="2c5eb-113">Escolha qualquer seleção opcional (em uma lista de seleções opcionais que você pode fazer neste ponto, muitas das quais podem ser deixadas com a configuração padrão para simplicidade).</span><span class="sxs-lookup"><span data-stu-id="2c5eb-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="2c5eb-114">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2c5eb-115">Você sempre pode voltar e editar essa regra mais tarde.</span><span class="sxs-lookup"><span data-stu-id="2c5eb-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="2c5eb-116">Para obter mais informações sobre como criar regras para criptografia, consulte Definir regras de fluxo de emails [para criptografar mensagens de email no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="2c5eb-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>
---
title: Exemplo da política de Anexo Seguro do Microsoft Defender para Office 365
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
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735371"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="13476-102">Exemplo da política de Anexo Seguro do Microsoft Defender para Office 365</span><span class="sxs-lookup"><span data-stu-id="13476-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="13476-103">Essas configurações habilitam uma política chamada *Sem atrasos* que entrega mensagens imediatamente e, em seguida, reatta anexos depois que eles são verificados:</span><span class="sxs-lookup"><span data-stu-id="13476-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="13476-104">**Nome**: Sem atrasos</span><span class="sxs-lookup"><span data-stu-id="13476-104">**Name**: No delays</span></span>
- <span data-ttu-id="13476-105">**Descrição**: entrega mensagens imediatamente e reatta anexos após a verificação.</span><span class="sxs-lookup"><span data-stu-id="13476-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="13476-106">**Resposta**: selecione a **opção Entrega** Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="13476-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="13476-107">Para obter mais informações, consulte [Entrega Dinâmica em Políticas de Anexos Seguros.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="13476-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="13476-108">**Seção Anexo de** redirecionamento: selecione a opção Habilitar redirecionamento **e** insira o endereço de email do administrador global do Microsoft 365, administrador de segurança ou analista de segurança que investigará anexos mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="13476-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="13476-109">**Seção Aplicado a:** Selecione **O domínio do destinatário é** e selecione seu domínio.</span><span class="sxs-lookup"><span data-stu-id="13476-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="13476-110">Selecione **adicionar** e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="13476-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="13476-111">Depois de terminar, selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="13476-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="13476-112">Para saber mais, confira [Anexos Seguros no Microsoft Defender para Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="13476-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>

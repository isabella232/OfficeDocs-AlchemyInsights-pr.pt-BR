---
title: Corrigir política de locatário (substituição de ação)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735355"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="ba727-102">Corrigir política de locatário (substituição de ação)</span><span class="sxs-lookup"><span data-stu-id="ba727-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="ba727-103">Uma política anti-spam em seu locatário afetou essa mensagem.</span><span class="sxs-lookup"><span data-stu-id="ba727-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="ba727-104">Para revisar a política, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ba727-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="ba727-105">Vá para o Centro de Conformidade e Segurança [& do Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)e vá para Política de Gerenciamento de Ameaças   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="ba727-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="ba727-106">Verifique se a origem **da** política indica o seguinte:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="ba727-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="ba727-107">Em caso afirmado, na **guia Personalizado,** verifique as configurações da política que afetou a mensagem.</span><span class="sxs-lookup"><span data-stu-id="ba727-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="ba727-108">É possível que as configurações **Padrão aplicadas** a todos os clientes da Proteção do Exchange Online afetaram a mensagem.</span><span class="sxs-lookup"><span data-stu-id="ba727-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="ba727-109">Para obter mais informações sobre como configurar políticas de filtro de spam, consulte [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="ba727-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>

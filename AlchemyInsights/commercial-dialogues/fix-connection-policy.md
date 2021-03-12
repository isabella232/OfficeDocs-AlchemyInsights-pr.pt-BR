---
title: Corrigir política de conexão
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735685"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="be28e-102">Corrigir política de conexão</span><span class="sxs-lookup"><span data-stu-id="be28e-102">Fix connection policy</span></span>

<span data-ttu-id="be28e-103">O email foi marcado como seguro e entregue à caixa de entrada do usuário porque o endereço IP de envio foi marcado como seguro na política filtro de conexão.</span><span class="sxs-lookup"><span data-stu-id="be28e-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="be28e-104">Para revisar a política, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="be28e-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="be28e-105">Vá para o Centro de Conformidade e Segurança [& do Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)e vá para Política de Gerenciamento de Ameaças   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="be28e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="be28e-106">Na guia **Personalizado,** selecione a política de filtro **de conexão** e selecione **Editar política**.</span><span class="sxs-lookup"><span data-stu-id="be28e-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="be28e-107">Revise a **lista de IDS.**</span><span class="sxs-lookup"><span data-stu-id="be28e-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="be28e-108">Veja se **a lista segura** está habilitada.</span><span class="sxs-lookup"><span data-stu-id="be28e-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="be28e-109">A Microsoft assina fontes terceirizadas de remetentes confiáveis.</span><span class="sxs-lookup"><span data-stu-id="be28e-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="be28e-110">Se **a lista segura** estiver habilitada, esses remetentes confiáveis não são marcados erroneamente como spam.</span><span class="sxs-lookup"><span data-stu-id="be28e-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="be28e-111">É recomendável selecionar essa opção, pois ela reduzirá o número de falsos positivos (emails que são classificados como spam) que você recebe.</span><span class="sxs-lookup"><span data-stu-id="be28e-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>

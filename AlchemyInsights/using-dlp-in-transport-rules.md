---
title: Usando DLP em regras de transporte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827204"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="e346b-102">Usando DLP em regras de transporte</span><span class="sxs-lookup"><span data-stu-id="e346b-102">Using DLP in transport rules</span></span>

<span data-ttu-id="e346b-103">Para integrar a Prevenção contra Perda de Dados (DLP) em um transporte existente, use a condição "**Se a mensagem contiver... Informações confidenciais**" na configuração da Regra de transporte.</span><span class="sxs-lookup"><span data-stu-id="e346b-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="e346b-104">**Para obter mais detalhes, confira:**</span><span class="sxs-lookup"><span data-stu-id="e346b-104">**For more details, see:**</span></span>

- <span data-ttu-id="e346b-105">Tipos de informações confidenciais da DLP integradas nas regras de transporte: [Integrar Regras de Informações Confidenciais](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="e346b-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="e346b-106">Você também pode testar a regra com ou sem teste de política usando o Modo de Teste na regra.</span><span class="sxs-lookup"><span data-stu-id="e346b-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="e346b-107">Você deve esperar 30 minutos após criar a regra antes de testá-la.</span><span class="sxs-lookup"><span data-stu-id="e346b-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="e346b-108">Confira [Testar regras de Fluxo/Transporte de Emails](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="e346b-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="e346b-109">**Observação**: Se você estiver tentando implementar uma nova política de DLP com regras de transporte no EAC, use [Políticas de DLP no Centro de Conformidade e Segurança](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e346b-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>

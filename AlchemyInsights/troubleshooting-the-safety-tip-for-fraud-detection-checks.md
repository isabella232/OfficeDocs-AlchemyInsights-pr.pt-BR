---
title: Solução de problemas da dica de segurança para verificações de detecção de fraude
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834719"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="d635b-102">Solução de problemas da dica de segurança para verificações de detecção de fraude</span><span class="sxs-lookup"><span data-stu-id="d635b-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="d635b-103">Se você estiver recebendo uma dica de segurança que diz "O remetente falhou nas verificações de detecção de fraude e pode não ser quem aparenta ser", o remetente falhou ao passar as verificações de autenticação DKIM ou SPF.</span><span class="sxs-lookup"><span data-stu-id="d635b-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="d635b-104">O melhor método para resolver isso é que o remetente autorize a si mesmo.</span><span class="sxs-lookup"><span data-stu-id="d635b-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="d635b-105">Se o remetente estiver enviando em seu nome, você precisará autorize-os adicionando o endereço IP do remetente ao seu registro SPF.</span><span class="sxs-lookup"><span data-stu-id="d635b-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="d635b-106">Consulte Solução de problemas da dica de segurança [vermelha (suspeita) para verificar verificações de detecção de fraude](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="d635b-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="d635b-107">Aqui estão alguns outros links que podem ajudar:</span><span class="sxs-lookup"><span data-stu-id="d635b-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="d635b-108">Como a Microsoft usa a estrutura de política de remetente (SPF) para impedir a spoofing</span><span class="sxs-lookup"><span data-stu-id="d635b-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="d635b-109">Configurar o SPF para ajudar a prevenir falsificação</span><span class="sxs-lookup"><span data-stu-id="d635b-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)

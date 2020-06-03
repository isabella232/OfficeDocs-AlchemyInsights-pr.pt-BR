---
title: Solucionando problemas de dica de segurança para verificações de detecção de fraude
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504971"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c3136-102">Solucionando problemas de dica de segurança para verificações de detecção de fraude</span><span class="sxs-lookup"><span data-stu-id="c3136-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c3136-103">Se você estiver obtendo uma dica de segurança que diz "o remetente falhou em nossas verificações de detecção de fraude e não pode ser quem parece ser", o remetente falhou ao passar por verificações de autenticação DKIM ou SPF.</span><span class="sxs-lookup"><span data-stu-id="c3136-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c3136-104">O melhor método para resolver isso é que o remetente autorize a si mesmos.</span><span class="sxs-lookup"><span data-stu-id="c3136-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c3136-105">Se o remetente estiver enviando em seu nome, você precisará autorizá-los adicionando o endereço IP do remetente ao seu registro SPF.</span><span class="sxs-lookup"><span data-stu-id="c3136-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c3136-106">Consulte [Solucionando problemas de dica de segurança vermelha (suspeita) para verificar a detecção de fraudes](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="c3136-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c3136-107">Veja alguns outros links que podem ajudar a:</span><span class="sxs-lookup"><span data-stu-id="c3136-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c3136-108">Como a Microsoft usa o Sender Policy Framework (SPF) para evitar falsificação</span><span class="sxs-lookup"><span data-stu-id="c3136-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c3136-109">Configure o SPF para ajudar a evitar falsificações</span><span class="sxs-lookup"><span data-stu-id="c3136-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)

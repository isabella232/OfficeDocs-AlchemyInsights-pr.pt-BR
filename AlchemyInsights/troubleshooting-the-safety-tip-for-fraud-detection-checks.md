---
title: Solucionando problemas de dica de segurança para verificações de detecção de fraude
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391197"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="e5142-102">Solucionando problemas de dica de segurança para verificações de detecção de fraude</span><span class="sxs-lookup"><span data-stu-id="e5142-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="e5142-103">Se você estiver obtendo uma dica de segurança que diz "o remetente falhou em nossas verificações de detecção de fraude e não pode ser quem parece ser", o remetente falhou ao passar por verificações de autenticação DKIM ou SPF.</span><span class="sxs-lookup"><span data-stu-id="e5142-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="e5142-104">O melhor método para resolver isso é que o remetente autorize a si mesmos.</span><span class="sxs-lookup"><span data-stu-id="e5142-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="e5142-105">Se o remetente estiver enviando em seu nome, você precisará autorizá-los adicionando o endereço IP do remetente ao seu registro SPF.</span><span class="sxs-lookup"><span data-stu-id="e5142-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="e5142-106">Consulte [solucionaNdo problemas de dica de segurança vermelha (suspeita) para verificar a detecção](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) de fraudes para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e5142-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="e5142-107">Veja alguns outros links que podem ajudar a:</span><span class="sxs-lookup"><span data-stu-id="e5142-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="e5142-108">Como o Office 365 usa o Sender Policy Framework (SPF) para evitar falsificação</span><span class="sxs-lookup"><span data-stu-id="e5142-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="e5142-109">Configurar a SPF no Office 365 para ajudar a evitar falsificação</span><span class="sxs-lookup"><span data-stu-id="e5142-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    


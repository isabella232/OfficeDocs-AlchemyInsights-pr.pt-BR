---
title: Verifica se a dica de segurança de detecção de fraude da solução de problemas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457055"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="3bb71-102">Verifica se a dica de segurança de detecção de fraude da solução de problemas</span><span class="sxs-lookup"><span data-stu-id="3bb71-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="3bb71-p101">Se você estiver obtendo uma dica de segurança que diz "o remetente falhou nossas verificações de detecção de fraude e pode não ser que eles parecem estar" e o remetente não passou por DKIM ou SPF verificações de autenticação. O melhor método para resolver esse problema é para o emissor autorizar a próprios. Se o remetente está enviando em seu nome, você precisará autorizá-los, adicionando o endereço IP do remetente ao seu registro SPF.</span><span class="sxs-lookup"><span data-stu-id="3bb71-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="3bb71-106">Para obter mais informações, consulte [verifica se a dica de vermelho safety (suspeitas) para detecção de fraude da solução de problemas](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="3bb71-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="3bb71-107">Aqui estão alguns outros links que podem ajudar:</span><span class="sxs-lookup"><span data-stu-id="3bb71-107">Here are some other links that can help:</span></span>
  
- <span data-ttu-id="3bb71-108">Como o Office 365 usa o Sender Policy Framework (SPF) para evitar a falsificação</span><span class="sxs-lookup"><span data-stu-id="3bb71-108">[How Office 365 uses sender policy framework (SPF) to prevent spoofing](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)</span></span>
    
- [<span data-ttu-id="3bb71-109">Configurar o SPF no Office 365 para ajudar a evitar falsificações</span><span class="sxs-lookup"><span data-stu-id="3bb71-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    


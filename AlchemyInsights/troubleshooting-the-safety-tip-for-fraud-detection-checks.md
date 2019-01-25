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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Verifica se a dica de segurança de detecção de fraude da solução de problemas

Se você estiver obtendo uma dica de segurança que diz "o remetente falhou nossas verificações de detecção de fraude e pode não ser que eles parecem estar" e o remetente não passou por DKIM ou SPF verificações de autenticação. O melhor método para resolver esse problema é para o emissor autorizar a próprios. Se o remetente está enviando em seu nome, você precisará autorizá-los, adicionando o endereço IP do remetente ao seu registro SPF.
  
Para obter mais informações, consulte [verifica se a dica de vermelho safety (suspeitas) para detecção de fraude da solução de problemas](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) . 
  
Aqui estão alguns outros links que podem ajudar:
  
- Como o Office 365 usa o Sender Policy Framework (SPF) para evitar a falsificação
    
- [Configurar o SPF no Office 365 para ajudar a evitar falsificações](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    


---
title: Verifica se a dica de segurança de detecção de fraude da solução de problemas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658103"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Verifica se a dica de segurança de detecção de fraude da solução de problemas



Se você estiver obtendo uma dica de segurança que diz "o remetente falhou nossas verificações de detecção de fraude e pode não ser que eles parecem estar" e o remetente não passou por DKIM ou SPF verificações de autenticação. O melhor método para resolver esse problema é para o emissor autorizar a próprios. Se o remetente está enviando em seu nome, você precisará autorizá-los, adicionando o endereço IP do remetente ao seu registro SPF.
  
Para obter mais informações, consulte [verifica se a dica de vermelho safety (suspeitas) para detecção de fraude da solução de problemas](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) . 
  
Aqui estão alguns outros links que podem ajudar:
  
- [Como o Office 365 usa a estrutura de política do remetente (SPF) para evitar a falsificação](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [Configurar o SPF no Office 365 para ajudar a evitar falsificações](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    


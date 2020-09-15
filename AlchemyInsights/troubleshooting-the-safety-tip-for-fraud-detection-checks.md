---
title: Solucionando problemas de dica de segurança para verificações de detecção de fraude
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658398"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Solucionando problemas de dica de segurança para verificações de detecção de fraude

Se você estiver obtendo uma dica de segurança que diz "o remetente falhou em nossas verificações de detecção de fraude e não pode ser quem parece ser", o remetente falhou ao passar por verificações de autenticação DKIM ou SPF. O melhor método para resolver isso é que o remetente autorize a si mesmos. Se o remetente estiver enviando em seu nome, você precisará autorizá-los adicionando o endereço IP do remetente ao seu registro SPF.
  
Consulte [Solucionando problemas de dica de segurança vermelha (suspeita) para verificar a detecção de fraudes](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obter mais informações.
  
Veja alguns outros links que podem ajudar a:
  
- [Como a Microsoft usa o Sender Policy Framework (SPF) para evitar falsificação](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configure o SPF para ajudar a evitar falsificações](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)

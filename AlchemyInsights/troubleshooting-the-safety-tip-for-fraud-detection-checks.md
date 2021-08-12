---
title: Solução de problemas dica de segurança verificações de detecção de fraude
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955954"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Solução de problemas dica de segurança verificações de detecção de fraude

Se você estiver recebendo um dica de segurança que diz "O remetente falhou nas verificações de detecção de fraude e pode não ser quem aparenta ser", o remetente falhou ao passar as verificações de autenticação DKIM ou SPF. O melhor método para resolver isso é que o remetente autorize a si mesmo. Se o remetente estiver enviando em seu nome, você precisará autorize-os adicionando o endereço IP do remetente ao seu registro SPF.
  
Consulte [Solução de problemas do sistema vermelho (suspeito) dica de segurança verificações de](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) detecção de fraude para obter mais informações.
  
Aqui estão alguns outros links que podem ajudar:
  
- [Como a Microsoft usa a estrutura de política de remetente (SPF) para impedir a spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurar o SPF para ajudar a prevenir falsificação](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)

---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506431"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrigir problemas de entrega de email com o código de erro 5.7.23

Verifique o registro DNS SPF do seu domínio em um SPF ou verificador de registro DNS disponível publicamente na Web.

Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do [pool de entrega de alto risco](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). As mensagens no pool de entrega de alto risco não passarão as verificações de SPF e, portanto, não serão aceitas pela organização de email de destino.

Se o problema persistir, talvez seja necessário entrar em contato com o administrador do host de email para o qual você está tentando enviar emails. Anote o erro externo detalhado disponível na mensagem de devolução. O suporte da Microsoft pode não conseguir assistência adicional.

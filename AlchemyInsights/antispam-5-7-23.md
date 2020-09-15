---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717313"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrigir problemas de entrega de email com o código de erro 5.7.23

Verifique o registro DNS SPF do seu domínio em um SPF ou verificador de registro DNS disponível publicamente na Web.

Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do [pool de entrega de alto risco](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). As mensagens no pool de entrega de alto risco não passarão as verificações de SPF e, portanto, não serão aceitas pela organização de email de destino.

Se o problema persistir, talvez seja necessário entrar em contato com o administrador do host de email para o qual você está tentando enviar emails. Anote o erro externo detalhado disponível na mensagem de devolução. O suporte da Microsoft pode não conseguir assistência adicional.

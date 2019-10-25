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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682026"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrigir problemas de entrega de email com o código de erro 5.7.23

Verifique o registro DNS SPF do seu domínio em um SPF ou verificador de registro DNS disponível publicamente na Web.

Verifique se a mensagem de saída não foi identificada como spam pelo Office 365 e encaminhada através do [pool de entrega de alto risco](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). As mensagens no pool de entrega de alto risco não passarão as verificações de SPF e, portanto, não serão aceitas pela organização de email de destino.

Se o problema persistir, talvez seja necessário entrar em contato com o administrador do host de email para o qual você está tentando enviar emails. Anote o erro externo detalhado disponível na mensagem de devolução.  O suporte do Office 365 pode não conseguir assistência adicional.
---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821399"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrigir problemas de entrega de email para o código de erro 5.7.23

Verifique o registro DNS do SPF para seu domínio em um SPF ou um verificador de registro DNS disponível publicamente na Web.

Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e roteada pelo Pool de Entrega de Alto [Risco.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) As mensagens no Pool de Entrega de Alto Risco não passarão verificações SPF e, portanto, não serão aceitas pela organização de email de destino.

Se o problema persistir, talvez seja necessário entrar em contato com o administrador do host de email para o qual você está tentando enviar emails. Anote o erro externo detalhado disponível na mensagem de rejeição. O suporte da Microsoft pode não ser capaz de ajudar ainda mais.

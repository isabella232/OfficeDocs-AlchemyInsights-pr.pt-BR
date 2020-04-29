---
title: Usando DLP em regras de transporte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915021"
---
# <a name="using-dlp-in-transport-rules"></a>Usando DLP em regras de transporte

Para integrar a Prevenção contra Perda de Dados (DLP) em um transporte existente, use a condição "**Se a mensagem contiver... Informações confidenciais**" na configuração da Regra de transporte.

**Para obter mais detalhes, confira:**

- Tipos de informações confidenciais da DLP integradas nas regras de transporte: [Integrar Regras de Informações Confidenciais](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Você também pode testar a regra com ou sem teste de política usando o Modo de Teste na regra.  Você deve esperar 30 minutos após criar a regra antes de testá-la.

- Confira [Testar regras de Fluxo/Transporte de Emails](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Observação**: Se você estiver tentando implementar uma nova política de DLP com regras de transporte no EAC, use [Políticas de DLP no Centro de Conformidade e Segurança](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).

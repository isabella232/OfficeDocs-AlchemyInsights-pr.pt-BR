---
title: 1332 OWA - regra (s) de caixa de entrada é não executá-lo para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275119"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Uma regra de caixa de entrada não está funcionando conforme o esperado

Verifique se as configurações a seguir:
  
- Pode ser redirecionada uma mensagem encaminhada ou respondida para automaticamente com base nas regras de caixa de entrada apenas uma vez. Uma regra de redirecionar (uma regra de caixa de entrada ou uma regra de fluxo de email, também conhecido como uma regra de transporte) pode adicionar um máximo de destinatários de encaminhamento de dez a uma mensagem. Para obter mais informações, consulte [limites de regra de diário, transporte e a caixa de entrada](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Regras de caixa de entrada não funcionam na caixa de correio de registro no diário alternativa. Para obter mais informações sobre a caixa de correio de registro no diário alternativa, consulte a [caixa de correio de registro no diário alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Para corrigir esses problemas, consulte [2829319 KB](https://support.microsoft.com/kb/2829319).
  
Se não aplicam os problemas anteriores, execute o relatório de diagnóstico de regra de caixa de entrada antes de escalonar o problema ao Microsoft Support:
  
1. Abra a caixa de correio no Outlook na web e clique em **configurações** \> **Opções** \> **Organizar email** \> **regras de caixa de entrada**.
    
2. Na parte inferior da página, clique em **se suas regras não estão funcionando clique aqui para gerar um relatório de diagnóstico**.
    


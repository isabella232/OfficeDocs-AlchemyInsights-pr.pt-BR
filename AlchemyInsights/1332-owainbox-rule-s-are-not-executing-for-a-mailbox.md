---
title: 1332 OWA - regra (s) de caixa de entrada é não executá-lo para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915792"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Uma regra de caixa de entrada não está funcionando conforme o esperado

Verifique se as configurações a seguir:
  
- Pode ser redirecionada uma mensagem encaminhada ou respondida para automaticamente com base nas regras de caixa de entrada apenas uma vez. Uma regra de redirecionar (uma regra de caixa de entrada ou uma regra de fluxo de email, também conhecido como uma regra de transporte) pode adicionar um máximo de destinatários de encaminhamento de dez a uma mensagem. Para obter mais informações, consulte [limites de regra de diário, transporte e a caixa de entrada](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Regras de caixa de entrada não funcionam na caixa de correio de registro no diário alternativa. Para obter mais informações sobre a caixa de correio de registro no diário alternativa, consulte a [caixa de correio de registro no diário alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Para corrigir esses problemas, consulte [2829319 KB](https://support.microsoft.com/kb/2829319).
  
Se não aplicam os problemas anteriores, execute o relatório de diagnóstico de regra de caixa de entrada antes de escalonar o problema ao Microsoft Support:
  
1. Abra a caixa de correio no Outlook na web e clique em **configurações** \> **Opções** \> **Organizar email** \> **regras de caixa de entrada**.
    
2. Na parte inferior da página, clique em **se suas regras não estão funcionando clique aqui para gerar um relatório de diagnóstico**.
    


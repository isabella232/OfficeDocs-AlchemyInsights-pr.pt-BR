---
title: 1332 OWA-regra (s) de caixa de entrada não estão sendo executadas para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858732"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Uma regra de caixa de entrada não funciona como esperado

Verifique as seguintes configurações:

- Uma mensagem pode ser redirecionada, encaminhada ou respondida automaticamente com base nas regras de caixa de entrada apenas uma vez. Uma regra de redirecionamento (uma regra de caixa de entrada ou regra de fluxo de emails, também conhecida como regra de transporte) pode adicionar no máximo dez destinatários de encaminhamento a uma mensagem. Para saber mais, confira [limites de regras de diário, transporte e caixa de entrada](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- As regras de caixa de entrada não funcionam na caixa de correio de registro em diário alternativa. Para obter mais informações sobre a caixa de correio de registro no diário alternativo, confira [caixa de correio de registro em diário alternativo](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Para corrigir esses problemas, confira [KB 2829319](https://support.microsoft.com/kb/2829319).

Se os problemas anteriores não se aplicarem, execute o relatório de diagnóstico da regra de caixa de entrada antes de escalonar o problema para o suporte da Microsoft:

1. Abra a caixa de correio no Outlook na Web e clique em **Opções** \> de **configurações** \> organizar **regras de caixa de entrada**de **email** \> .

2. Na parte inferior da página, clique em **se suas regras não estiverem funcionando, clique aqui para gerar um relatório de diagnóstico**.

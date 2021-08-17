---
title: 726 Bloqueando o encaminhamento de email
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059620"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloquear ou desbloquear o encaminhamento de email

Para habilitar ou desabilitar o encaminhamento de email para uma caixa de correio específica, consulte [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

No nível do locatário, o controle do encaminhamento externo é feito usando a política de spam de saída. Você pode verificar a política de filtro [](https://protection.office.com/antispam) de spam de saída do Centro de Conformidade e Segurança aqui ou usando o comando [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Se você estiver recebendo o seguinte erro: **"550 5.7.520 Access negado,** Sua organização não permitirá o encaminhamento externo" , verifique se a política está configurada para habilitar o Encaminhamento Automático Externo.

**Observação:** É recomendável manter a Autoforward Externa desabilitada em sua política de filtro de spam de saída padrão e habilita-la somente para os usuários que precisam de encaminhamento externo criando uma política personalizada para esses usuários. Você pode ler mais em [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
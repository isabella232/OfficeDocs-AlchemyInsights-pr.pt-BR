---
title: Bloquear ou desbloquear o encaminhamento automático de email externo
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315862"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Bloquear ou desbloquear o encaminhamento automático de email eterno

Para habilitar ou desabilitar o encaminhamento de email para uma caixa de correio específica, consulte [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Os administradores podem controlar o encaminhamento externo para a organização usando [políticas de spam de saída.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Você gerencia políticas de spam de saída no portal Microsoft 365 Defender em ou usando o <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) no Exchange Online PowerShell.

Se você receber o seguinte erro: **"550 5.7.520 Access negado,** Sua organização não permitirá o encaminhamento externo" , certifique-se de que a política está configurada para habilitar mensagens externas encaminhadas automaticamente.

**Observação**: recomendamos o valor padrão  **Automatic -** Sistema controlado para a configuração de regras de encaminhamento automático em sua política de filtro de spam de saída padrão (o encaminhamento externo automático está bloqueado; o encaminhamento automático interno ainda funciona). Você deve criar políticas personalizadas de filtro de spam de saída e usar o valor **Ativado -** O encaminhamento só é habilitado para usuários que precisam de encaminhamento automático de email externo. Para obter mais informações, consulte [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).

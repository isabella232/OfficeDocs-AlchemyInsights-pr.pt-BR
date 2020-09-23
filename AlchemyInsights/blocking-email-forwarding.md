---
title: 726 bloquear o encaminhamento de email
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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219843"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Bloqueando ou desbloqueando o encaminhamento de email

Para habilitar ou desabilitar o encaminhamento de emails para uma caixa de correio específica, confira [Configurar o encaminhamento de email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

No nível do locatário, o controle de encaminhamento externo é feito usando a política antispam de saída. Se ele estiver definido como desativado ou automático, ele poderá bloquear o encaminhamento de emails com o erro "550 5.7.520 acesso negado, sua organização não permitir encaminhamento externo". Subsequentemente, se o encaminhamento estiver definido para ser bloqueado, esse será o erro que os usuários verão.

Se o encaminhamento estiver bloqueado, certifique-se de que a política está configurada para habilitar o avanço avançado externo. Você pode verificar a política de filtro de spam de saída do centro de segurança e conformidade ou executando o comando Get-HostedOutboundSpamFilterPolicy | nome da FL, AutoForwardingMode. Se você quiser configurar o bloqueio de avanços, o mesmo comando informará o estado da política agora.

Observação: é recomendável manter o encaminhamento automático externo desabilitado na política de filtro de spam de saída padrão e habilitá-lo somente para os usuários que precisam de encaminhamento externo criando uma política personalizada para esses usuários. Você pode ler mais sobre como [Configurar o encaminhamento de email externo no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
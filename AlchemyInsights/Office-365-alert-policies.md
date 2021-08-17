---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312675"
---
# <a name="alert-policies"></a>Políticas de alerta

Microsoft 365 contém políticas [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) de alerta padrão que disparam alertas para organizações com uma assinatura do Microsoft 365 Enterprise ou Microsoft 365 US Government E1/G1, E3/G3 ou E5/G5. Portanto, os administradores podem receber uma notificação de email de alerta enviada pelo Office365Alerts@microsoft.com com uma linha de assunto como "Um alerta de baixa gravidade: nome da política *de alerta".* As notificações de alerta são enviadas quando alertas são disparados para atividades comuns, como quando os usuários:

- Criar regras de caixa de entrada que encaminham emails.
- Atribua permissões à caixa de correio.
- Compartilhar ou excluir um grande número de arquivos SharePoint compartilhamento de arquivos.
- Crie pesquisas de Descobertas EDiscovery e exporte resultados de pesquisa.

Para revisar e agir em um alerta:

1. Siga uma das seguintes etapas:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para **Alertas**. Ou, para ir diretamente para a página **Alertas,** use <https://compliance.microsoft.com/compliancealerts> .
   - No portal Microsoft 365 Defender em , vá para <https://security.microsoft.com> **Incidentes &** \> **alertas**. Ou, para ir diretamente para a página **Alertas,** use <https://security.microsoft.com/alerts> .
2. Clique em um alerta para exibir uma página de sobrevoo com informações sobre o alerta.

Você pode tomar medidas em um alerta, como [remover uma regra de caixa de entrada suspeita.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Ou você pode simplesmente fechar o alerta clicando em **Resolver** na página de sobrevoo de alerta.

Para obter mais informações sobre como configurar e gerenciar políticas de alerta, consulte  [este artigo](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**Importante:** alertar as notificações de email da Microsoft nunca solicitará que você faça o seguinte:

- Fornecer uma senha
- Verificar os detalhes de segurança da sua conta
- Re-autenticar a si mesmo

Se você receber uma mensagem de email com esses tipos de solicitações, ela não foi enviada pela Microsoft e deve ser considerada uma fraude de phishing. Se você receber uma mensagem com esses tipos de solicitações, [reporte a mensagem à Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

---
title: Identificar encaminhamento de email externo em caixas de correio em logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331147"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o encaminhamento de email externo é configurado em caixas de correio

Quando um Microsoft 365 configura o encaminhamento de email externo em uma caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox.** Você pode ver a atividade usando a pesquisa de log de auditoria. Veja como fazer isso.

1. Siga uma das seguintes etapas:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com>, vá para **Soluções** \> **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://compliance.microsoft.com/auditlogsearch>.
   - No portal do Microsoft 365 Defender em <https://security.microsoft.com>, vá para **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://sip.security.microsoft.com/auditlogsearch>.

2. Na página **Auditoria**, verifique se a guia **Pesquisa** está selecionada e defina as seguintes configurações:
   - Selecione o intervalo de data/hora nas caixas **Iniciar** **e** Fim.
   - Verifique se **a caixa Atividades** contém Mostrar resultados de todas as **atividades**.

3. Ao concluir, clique em **Pesquisar**. As atividades aparecem na nova página **Pesquisa de auditoria**.

4. Nos resultados, clique em **Filtrar resultados** e digite **Set-Mailbox** na caixa de filtro de atividade.

5. Selecione um registro de auditoria nos resultados. No **sobremenu de** Detalhes, clique **em Mais informações.** Você precisa ver os detalhes de cada registro de auditoria para determinar se a atividade está relacionada ao encaminhamento de email.

   - **ObjectId**: o valor de alias da caixa de correio que foi modificada.
   - **Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de email de destino.
   - **UserId**: o usuário que configurou o encaminhamento de email na caixa de correio no **campo ObjectId.**

Para obter mais informações, [consulte Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).

---
title: Identificar o encaminhamento de emails externos em caixas de correio em logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508940"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o encaminhamento de email externo é configurado em caixas de correio

Quando um usuário do Microsoft 365 configura o encaminhamento de email externo em uma caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox** . Você pode ver a atividade usando a pesquisa de log de auditoria no centro de conformidade de & de segurança.

1. Faça logon no [centro de conformidade & segurança da Microsoft 365](https://protection.office.com/).

2. Vá para a **Search**  >  página**pesquisa de log de auditoria** de pesquisa.

3. Selecione o intervalo de datas nos campos **data de início** e data de **término** . Não é necessário especificar um nome de usuário. Verifique se o campo **atividades** está definido para **Mostrar os resultados de todas as atividades**.

4. Clique em **Pesquisar**.

Nos resultados, clique em **filtrar resultados** e digite **Set-Mailbox** na caixa filtro de atividade. Selecione um registro de auditoria nos resultados. No submenu **detalhes** , clique em **mais informações**. Você precisa examinar os detalhes de cada registro de auditoria para determinar se a atividade está relacionada ao encaminhamento de email.

- **ObjectID**: o valor do alias da caixa de correio que foi modificado.

- **Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de email de destino.

- **Userid**: o usuário que configurou o encaminhamento de emails na caixa de correio no campo **ObjectID** .

Para obter mais informações, consulte [determinando quem configurou o encaminhamento de email para uma caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).

---
title: Identificar o encaminhamento de emails externos em caixas de correio em logs de auditoria
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417200"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o encaminhamento de email externo é configurado em caixas de correio

Quando um usuário configura o encaminhamento de email externo em uma caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox** . Você pode ver a atividade usando a pesquisa de log de auditoria no centro de conformidade do & de segurança.

1. Faça logon no [centro de conformidade do & de segurança do Office 365](https://protection.office.com/)

2. Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.

3. Selecione o intervalo de datas nos campos **data de início** e data de **término** . Não é necessário especificar um nome de usuário. Verifique se o campo **atividades** está definido para **Mostrar os resultados de todas as atividades**.

4. Clique em **Pesquisar**.

Nos resultados, clique em **filtrar resultados** e digite **Set-Mailbox** na caixa filtro de atividade. Selecione um registro de auditoria nos resultados. No submenu **detalhes** , clique em **mais informações**. Você precisa examinar os detalhes de cada registro de auditoria para determinar se a atividade está relacionada ao encaminhamento de email.

- **ObjectID**: o valor do alias da caixa de correio que foi modificado.

- **Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de email de destino.

- **Userid**: o usuário que configurou o encaminhamento de emails na caixa de correio no campo **ObjectID** .

Para obter mais informações, consulte [determinando quem configurou o encaminhamento de email para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).

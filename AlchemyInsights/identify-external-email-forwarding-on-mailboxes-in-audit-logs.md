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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028714"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o encaminhamento de email externo é configurado em caixas de correio

Quando um Microsoft 365 configura o encaminhamento de email externo em uma caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox.** Você pode ver a atividade usando a pesquisa de log de auditoria no Centro de Conformidade & Segurança.

1. Faça logoff no [Centro de Conformidade Microsoft 365 .](https://protection.office.com/)

2. Vá para a **página de pesquisa** de log de Auditoria  >  **de** Pesquisa.

3. Selecione o intervalo de datas nos campos **Data de** início e **Data de** término. Não é necessário especificar um nome de usuário. Verifique se **o campo Atividades** está definido como Mostrar resultados de todas as **atividades.**

4. Clique em **Pesquisar**.

Nos resultados, clique em **Filtrar Resultados** e digite **Set-Mailbox** na caixa de filtro de atividade. Selecione um registro de auditoria nos resultados. No **sobremenu de** Detalhes, clique **em Mais informações.** Você precisa ver os detalhes de cada registro de auditoria para determinar se a atividade está relacionada ao encaminhamento de email.

- **ObjectId**: o valor de alias da caixa de correio que foi modificada.

- **Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de email de destino.

- **UserId**: o usuário que configurou o encaminhamento de email na caixa de correio no **campo ObjectId.**

Para obter mais informações, [consulte Determining who set up email forwarding for a mailbox](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).

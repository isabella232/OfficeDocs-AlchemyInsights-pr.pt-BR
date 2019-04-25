---
title: Identificar a atividade da regra de caixa de entrada nos logs de auditoria
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417235"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar a atividade da regra de caixa de entrada nos logs de auditoria

Você pode usar a pesquisa de log de auditoria no centro de conformidade do & de segurança para exibir eventos de regra de caixa de entrada (criando, modificando e excluindo regras de caixa de entrada).

1. Faça logon no [centro de conformidade do & de segurança do Office 365](https://protection.office.com/)

2. Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.

3. Selecione o intervalo de datas nos campos **data de início** e data de **término** .

4. Em **atividades de caixa de correio do Exchange**, verifique se o campo **atividades** está definido como **New-InboxRule criar/modificar/habilitar/desabilitar regra de caixa de entrada**.

5. Clique em **Pesquisar**.

Nos resultados, selecione um registro de auditoria. No submenu detalhes, clique em **mais informações**. As informações sobre as configurações da regra de caixa de entrada são exibidas no campo **parâmetros** .

Para obter mais informações, consulte [determinando se um usuário criou uma regra de caixa de entrada](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)

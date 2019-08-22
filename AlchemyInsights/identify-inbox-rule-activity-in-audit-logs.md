---
title: Identificar a atividade da regra de caixa de entrada nos logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539125"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar a atividade da regra de caixa de entrada nos logs de auditoria

Você pode usar a pesquisa de log de auditoria no centro de conformidade & segurança do Office 365 para exibir eventos de regra de caixa de entrada (criando, modificando e excluindo regras de caixa de entrada).

1. Faça logon no [centro de conformidade & segurança do Office 365](https://protection.office.com/).

2. Vá para a página**pesquisa de log de auditoria** de **pesquisa** > .

3. Selecione o intervalo de datas nos campos **data de início** e data de **término** .

4. Em **atividades de caixa de correio do Exchange**, verifique se o campo **atividades** está definido como **New-InboxRule criar/modificar/habilitar/desabilitar regra de caixa de entrada**.

5. Clique em **Pesquisar**.

Nos resultados, selecione um registro de auditoria. No submenu detalhes, clique em **mais informações**. As informações sobre as configurações da regra de caixa de entrada são exibidas no campo **parâmetros** .

Para obter mais informações, consulte [determinando se um usuário criou uma regra de caixa de entrada](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)

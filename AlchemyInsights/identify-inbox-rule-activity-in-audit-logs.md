---
title: Identificar a atividade da regra de caixa de entrada nos logs de auditoria
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779039"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar a atividade da regra de caixa de entrada nos logs de auditoria

Você pode usar a pesquisa de log de auditoria no centro de conformidade & segurança da Microsoft 365 para exibir eventos de regra de caixa de entrada (criando, modificando e excluindo regras de caixa de entrada).

1. Faça logon no [centro de conformidade & segurança da Microsoft 365](https://protection.office.com/).

2. Vá para a **Search**  >  página**pesquisa de log de auditoria** de pesquisa.

3. Selecione o intervalo de datas nos campos **data de início** e data de **término** .

4. Em **atividades de caixa de correio do Exchange**, verifique se o campo **atividades** está definido como **New-InboxRule criar/modificar/habilitar/desabilitar regra de caixa de entrada**.

5. Clique em **Pesquisar**.

Nos resultados, selecione um registro de auditoria. No submenu detalhes, clique em **mais informações**. As informações sobre as configurações da regra de caixa de entrada são exibidas no campo **parâmetros** .

Para obter mais informações, consulte [determinando se um usuário criou uma regra de caixa de entrada](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)

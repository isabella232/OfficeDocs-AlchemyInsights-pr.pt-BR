---
title: Identificar atividade de regra de caixa de entrada em logs de auditoria
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
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976853"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar atividade de regra de caixa de entrada em logs de auditoria

Você pode usar a pesquisa de log de auditoria no Centro de Conformidade Microsoft 365 Segurança & para exibir eventos de regra de caixa de entrada (criação, modificação e exclusão de regras de caixa de entrada).

1. Faça logoff no [Centro de Conformidade Microsoft 365 .](https://protection.office.com/)

2. Vá para a **página de pesquisa** de log de Auditoria  >  **de** Pesquisa.

3. Selecione o intervalo de datas nos campos **Data de** início e **Data de** término.

4. Em **Exchange Atividades** de Caixa de Correio, verifique se o campo **Atividades** está definido como **New-InboxRule Create/modify/enable/disable inbox rule**.

5. Clique em **Pesquisar**.

Nos resultados, selecione um registro de auditoria. No sobremenu de detalhes, clique **em Mais Informações.** As informações sobre as configurações de regra de caixa de entrada são exibidas no **campo Parâmetros.**

Para obter mais informações, [consulte Determining if a user created an inbox rule](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)

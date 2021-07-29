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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630165"
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

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
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891283"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar atividade de regra de caixa de entrada em logs de auditoria

Você pode usar a pesquisa de log de auditoria no Centro de conformidade do Microsoft 365 para exibir eventos de regra de caixa de entrada (criando, modificando e excluindo regras de caixa de entrada).

1. Faça o seguinte:
   - Na Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para **Auditoria de** \> **Soluções.** Ou, para ir diretamente para a página **Auditoria,** use <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender em <https://security.microsoft.com> , vá para **Auditoria**. Ou, para ir diretamente para a página **Auditoria,** use <https://security.microsoft.com/auditlogsearch> .

2. Na guia **Pesquisa** da página **Auditoria,** configure as seguintes configurações:
   - **Intervalo de data e hora**: Selecione o intervalo de data/hora nas caixas **Iniciar** **e** Fim.
   - **Atividades**: selecione um ou mais dos seguintes valores:
     - **Regra de caixa de entrada New-InboxRule Create Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Atualizar regras de caixa de entrada Outlook cliente**

3. Quando terminar, clique em **Pesquisar**. As atividades aparecem na nova página **de pesquisa auditoria.**

4. Selecione uma atividade nos resultados para abrir o sobremenu de detalhes. As informações sobre as configurações de regra de caixa de entrada são exibidas no **campo Parâmetros.**

Para obter mais informações, [consulte Determining if a user created an inbox rule](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).

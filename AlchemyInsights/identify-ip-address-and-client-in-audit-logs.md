---
title: Identificar endereço IP e cliente em logs de auditoria
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313007"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar endereço IP e cliente em logs de auditoria

O endereço IP que corresponde a uma atividade por um Microsoft 365 ou administrador é mostrado nos Logs de Auditoria. As informações do cliente também são registradas. Aqui estão as etapas para identificar essas informações

1. Faça logoff no [Centro de Conformidade Microsoft 365 .](https://protection.office.com/)

2. Vá para a **página de pesquisa** de log de Auditoria  >  **de** Pesquisa.

   Se você estiver interessado em uma atividade específica, selecione-a na **lista Atividades.** Caso não seja, todas as atividades serão retornadas para o usuário selecionado (configuração padrão).

   **Observação:** determinadas atividades podem não estar disponíveis no menu **Atividades;** no entanto, esses itens de auditoria serão retornados se **Mostrar Resultados de todas as** atividades estiver selecionado (configuração padrão).

3. Especifique o nome de usuário no campo **Usuários,** selecione o intervalo de datas apropriado para a atividade e clique em **Pesquisar**.

Nos resultados, você pode ver o endereço IP dessa atividade no painel de resultados. Selecione o registro de auditoria para  ver informações detalhadas no sobremenu de Detalhes (por exemplo, Cliente, Usuário que realizou a ação, etc.).

Para obter mais informações, consulte [Localizar o endereço IP do computador usado para acessar uma conta comprometida.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)

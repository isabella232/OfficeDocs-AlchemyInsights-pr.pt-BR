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
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668298"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar endereço IP e cliente em logs de auditoria

O endereço IP que corresponde a uma atividade por um usuário ou administrador do Microsoft 365 é mostrado nos logs de auditoria. As informações do cliente também são registradas. Aqui estão as etapas para identificar essas informações

1. Faça logon no [centro de conformidade & segurança da Microsoft 365](https://protection.office.com/).

2. Vá para a **Search**  >  página**pesquisa de log de auditoria** de pesquisa.

   Se você estiver interessado em uma atividade específica, selecione-a na lista de **atividades** . Caso contrário, todas as atividades serão retornadas para o usuário selecionado (configuração padrão).

   **Observação**: determinadas atividades podem não estar disponíveis no menu **atividades** ; no entanto, esses itens de auditoria serão retornados se **Mostrar resultados de todas as atividades** for selecionado (configuração padrão).

3. Especifique o nome de usuário no campo **usuários** , selecione o intervalo de datas apropriado para a atividade e clique em **Pesquisar**.

Nos resultados, você pode ver o endereço IP dessa atividade no painel de resultados. Selecione o registro de auditoria para ver informações detalhadas no submenu **detalhes** (por exemplo, cliente, usuário que executou a ação, etc.).

Para obter mais informações, consulte [localizar o endereço IP do computador usado para acessar uma conta comprometida](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).

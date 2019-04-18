---
title: Identificar endereço IP e cliente em logs de auditoria
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909023"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar endereço IP e cliente em logs de auditoria

O endereço IP que corresponde a uma atividade por um usuário ou administrador é mostrado nos logs de auditoria. As informações do cliente também são registradas. Aqui estão as etapas para identificar essas informações

1. Faça logon no [centro de conformidade do & de segurança do Office 365](https://protection.office.com/)

2. Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.

   Se você estiver interessado em uma atividade específica, selecione-a na lista de **atividades** . Caso contrário, todas as atividades serão retornadas para o usuário selecionado (configuração padrão).

   **Observação**: determinadas atividades podem não estar disponíveis no menu **atividades** ; no entanto, esses itens de auditoria serão retornados se **Mostrar resultados de todas as atividades** for selecionado (configuração padrão).

3. Especifique o nome de usuário no campo **usuários** , selecione o intervalo de datas apropriado para a atividade e clique em **Pesquisar**.

Nos resultados, você pode ver o endereço IP dessa atividade no painel de resultados. Selecione o registro de auditoria para ver informações detalhadas no submenu **detalhes** (por exemplo, cliente, usuário que executou a ação, etc.).

Para obter mais informações, consulte [localizar o endereço IP do computador usado para acessar uma conta comprometida](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).

---
title: Encontre o endereço IP no log de auditoria
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017120"
---
# <a name="find-the-ip-address-in-audit-log"></a>Encontre o endereço IP no log de auditoria

1. O endereço IP que corresponde a uma atividade executada por um usuário ou administrador é mostrado nos logs de auditoria. As informações do cliente também são registradas. Veja como identificar o endereço IP:

1. Vá para o centro de conformidade [Office 365 segurança & segurança.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione **Pesquisa de** log de auditoria de  >  **[pesquisa](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver habilitado, os resultados da pesquisa não poderão puxar dados de datas anteriores.
1. Se você estiver interessado em uma atividade específica, selecione-a na lista **Atividades;** caso contrário, por padrão, todas as atividades serão retornadas para o usuário selecionado. Observe que determinadas atividades podem não estar disponíveis para seleção no menu **Atividades;** no entanto, esses itens de auditoria serão retornados se **Mostrar resultados de todas as atividades** estiver selecionado (configuração padrão).
1. Especifique o intervalo de datas e, no campo **Usuários,** selecione o nome de usuário do usuário que você deseja investigar.
1. Selecione **Pesquisar**. As atividades são exibidas em **Resultados**. Você pode ver o endereço IP de cada atividade.
1. Para exibir detalhes, selecione uma atividade e selecione **Mais Informações**.

Para saber mais, confira Pesquisar o log [de auditoria Office 365 para solucionar problemas de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)
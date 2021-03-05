---
title: Encontrar eventos executados em regras de caixa de entrada
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464348"
---
# <a name="find-events-performed-on-inbox-rules"></a>Encontrar eventos executados em regras de caixa de entrada

Quando as regras de caixa de entrada são criadas, alteradas ou excluídas, os eventos são gravados no log de auditoria. Veja como revisá-los:

1. Vá para o Centro de Conformidade e Segurança [& do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione Pesquisar > pesquisa de log de auditoria.

    > [!NOTE]
    > Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.
1. Selecione o campo Atividades e encontre atividades de caixa de correio do Exchange e selecione criar New-InboxRule regra de caixa de entrada do Outlook Web App. Quando terminar, clique fora do painel para minimizar o painel Atividades.
1. Especifique o intervalo de datas e, em seguida, no campo Usuários, selecione o nome de usuário do usuário que você deseja investigar. Você pode selecionar mais de um usuário por vez.
1. Selecione Pesquisar. As atividades aparecem em Resultados.
1. Para exibir detalhes, selecione uma atividade e selecione Mais Informações. Na seção Parâmetros, você pode ver o nome da regra, das condições definidas e das ações que a regra tomará.

Para saber mais, confira Pesquisar o log de auditoria do Office 365 para solucionar problemas de cenários comuns.
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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058638"
---
# <a name="find-events-performed-on-inbox-rules"></a>Encontrar eventos executados em regras de caixa de entrada

Quando as regras de caixa de entrada são criadas, alteradas ou excluídas, os eventos são gravados no log de auditoria. Veja como revisá-los:

1. Vá para o centro de conformidade [Office 365 segurança & segurança.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione Pesquisar > pesquisa de log de auditoria.

    > [!NOTE]
    > Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.
1. Selecione o campo Atividades e encontre Exchange de caixa de correio e selecione criar New-InboxRule regra de caixa de entrada do Outlook Web App. Quando terminar, clique fora do painel para minimizar o painel Atividades.
1. Especifique o intervalo de datas e, em seguida, no campo Usuários, selecione o nome de usuário do usuário que você deseja investigar. Você pode selecionar mais de um usuário por vez.
1. Selecione Pesquisar. As atividades são exibidas em Resultados.
1. Para exibir detalhes, selecione uma atividade e selecione Mais Informações. Na seção Parâmetros, você pode ver o nome da regra, das condições definidas e das ações que a regra tomará.

Para saber mais, confira Pesquisar o log de Office 365 de auditoria para solucionar problemas de cenários comuns.
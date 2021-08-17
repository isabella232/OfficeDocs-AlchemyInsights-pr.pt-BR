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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313487"
---
# <a name="find-events-performed-on-inbox-rules"></a>Encontrar eventos executados em regras de caixa de entrada

Quando as regras de caixa de entrada são criadas, alteradas ou excluídas, os eventos são gravados no log de auditoria. Veja como revisá-los:

1. Faça uma das seguintes ações:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com>, vá para **Soluções** \> **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://compliance.microsoft.com/auditlogsearch>.
   - No portal do Microsoft 365 Defender em <https://security.microsoft.com>, vá para **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://security.microsoft.com/auditlogsearch>.

    **Observação**: se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.
1. Selecione o campo Atividades e encontre Exchange de caixa de correio e selecione criar New-InboxRule regra de caixa de entrada do Outlook Web App. Quando terminar, clique fora do painel para minimizar o painel Atividades.
1. Especifique o intervalo de datas e, em seguida, no campo Usuários, selecione o nome de usuário do usuário que você deseja investigar. Você pode selecionar mais de um usuário por vez.
1. Selecione Pesquisar. As atividades são exibidas em Resultados.
1. Para exibir detalhes, selecione uma atividade e selecione Mais Informações. Na seção Parâmetros, você pode ver o nome da regra, das condições definidas e das ações que a regra tomará.

2. Na guia **Pesquisa** da página **Auditoria,** configure as seguintes configurações:
   - **Intervalo de data e hora**: Selecione o intervalo de data/hora nas caixas **Iniciar** e **Fim**.
   - **Atividades**: Selecione **Regra de caixa de entrada Criar** Nova Caixa de Entrada Outlook Web App

3. Ao concluir, clique em **Pesquisar**. As atividades aparecem na nova página **Pesquisa de auditoria**.

4. Selecione uma atividade nos resultados para abrir o sobremenu de detalhes. Na seção **Parâmetros,** você pode ver o nome da regra, das condições definidas e das ações que a regra tomará.

Para saber mais, confira [Pesquisar o log de auditoria para investigar problemas comuns de suporte.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)

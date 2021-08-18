---
title: Investigar todas as atividades dos usuários
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332331"
---
# <a name="investigate-all-the-users-activities"></a>Investigar todas as atividades dos usuários

Veja como fazer isso:

1. Faça uma das seguintes ações:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com>, vá para **Soluções** \> **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://compliance.microsoft.com/auditlogsearch>.
   - No portal do Microsoft 365 Defender em <https://security.microsoft.com>, vá para **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://security.microsoft.com/auditlogsearch>.

    **Observação**: se você vir um aviso de que precisa ativar o recurso, vá em frente e a ligue agora. Se o recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.

2. Na guia **Pesquisa** da página **Auditoria,** configure as seguintes configurações:
   - **Intervalo de data e hora**: Selecione o intervalo de data/hora nas caixas **Iniciar** e **Fim**.
   - **Atividades**: Se você estiver interessado em uma atividade específica, selecione-a na lista; caso contrário, o valor padrão **Mostrar resultados de todas as atividades** retorna todas as atividades.
   - **Usuários**: aceite o valor padrão em branco para retornar resultados para todos os usuários, ou insira um ou mais usuários.

3. Ao concluir, clique em **Pesquisar**. As atividades aparecem na nova página **Pesquisa de auditoria**. Você verá o **endereço IP,** **o** usuário e o **nome de** atividade.

4. Para baixar os resultados, selecione **Exportar** \> **Baixar todos os resultados**.

5. Selecione uma atividade nos resultados para abrir o sobremenu de detalhes.

Para saber mais, confira [Pesquisar o log de auditoria para investigar problemas comuns de suporte.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)

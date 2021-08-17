---
title: Recuperar os logs de auditoria
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: 6ca61775d18fb5501911fb3334ef499ff1f06a6b42634367eaf546fc322f822c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889634"
---
# <a name="retrieve-the-audit-logs"></a>Recuperar os logs de auditoria

Quando você abre o log de auditoria pela primeira vez, ele está vazio. Você tem que fazer uma pesquisa para ver seu conteúdo. Veja como fazer uma pesquisa geral de todas as atividades:

1. Siga uma das seguintes etapas:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com>, vá para **Soluções** \> **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://compliance.microsoft.com/auditlogsearch>.
   - No portal do Microsoft 365 Defender em <https://security.microsoft.com>, vá para **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://sip.security.microsoft.com/auditlogsearch>.

2. Na página **Auditoria**, verifique se a guia **Pesquisa** está selecionada e defina as seguintes configurações:
   - **Intervalo de data e hora**: Selecione o intervalo de data/hora nas caixas **Iniciar** e **Fim**.
   - **Atividades**: Verifique se **Mostrar resultados de todas atividades** está selecionado.
   - **Usuários**: aceite o valor padrão em branco para retornar resultados para todos os usuários, ou insira um ou mais usuários.

3. Ao concluir, clique em **Pesquisar**. As atividades aparecem na nova página **Pesquisa de auditoria**.

4. Nos resultados, clique em **Filtrar resultados** e digite **Set-Mailbox** na caixa de filtro de atividade.

5. Selecione um registro de auditoria nos resultados. No submenu **Detalhes**, clique em **Mais informações** para exibir mais informações, como Cliente, Usuário que executou a ação e assim por diante.

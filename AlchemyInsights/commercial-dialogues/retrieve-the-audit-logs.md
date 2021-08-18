---
title: Recuperar os logs de auditoria
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
ms.openlocfilehash: 88d28898923c1381c001c15445da90901b7e8761
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320431"
---
# <a name="retrieve-the-audit-logs"></a>Recuperar os logs de auditoria

Quando você abrir o log de auditoria pela primeira vez, ele estará vazio. Você tem que fazer uma pesquisa para ver seu conteúdo. Veja como fazer uma pesquisa geral de todas as atividades:

1. Faça uma das seguintes ações:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com>, vá para **Soluções** \> **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://compliance.microsoft.com/auditlogsearch>.
   - No portal do Microsoft 365 Defender em <https://security.microsoft.com>, vá para **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://security.microsoft.com/auditlogsearch>.

2. Na guia **Pesquisa** da página **Auditoria,** configure as seguintes configurações:
   - **Intervalo de data e hora**: Selecione o intervalo de data/hora nas caixas **Iniciar** e **Fim**.
   - **Atividades**: Verifique se **Mostrar resultados de todas atividades** está selecionado.
   - **Usuários**: aceite o valor padrão em branco para retornar resultados para todos os usuários, ou insira um ou mais usuários.

3. Ao concluir, clique em **Pesquisar**. As atividades aparecem na nova página **Pesquisa de auditoria**.

4. Selecione uma atividade nos resultados para abrir o sobremenu de detalhes. Você verá mais informações como Cliente, Usuário que realizou a ação, etc.

Para saber mais, confira [Pesquisar o log de auditoria para investigar problemas comuns de suporte.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)

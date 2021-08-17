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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303565"
---
# <a name="find-the-ip-address-in-audit-log"></a>Encontre o endereço IP no log de auditoria

O endereço IP que corresponde a uma atividade executada por um usuário ou administrador é mostrado nos logs de auditoria. As informações do cliente também são registradas. Veja como identificar o endereço IP:

1. Faça uma das seguintes ações:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com>, vá para **Soluções** \> **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://compliance.microsoft.com/auditlogsearch>.
   - No portal do Microsoft 365 Defender em <https://security.microsoft.com>, vá para **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://security.microsoft.com/auditlogsearch>.

    **Observação**: se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver habilitado, os resultados da pesquisa não poderão puxar dados de datas anteriores.

2. Na página **Auditoria**, verifique se a guia **Pesquisa** está selecionada e defina as seguintes configurações:
   - **Intervalo de data e hora**: Selecione o intervalo de data/hora nas caixas **Iniciar** e **Fim**.
   - **Atividades**: Se você estiver interessado em uma atividade específica, selecione-a na lista; caso contrário, o valor padrão **Mostrar resultados de todas as atividades** retornará todas as atividades.. Observe que determinadas atividades podem não estar disponíveis para seleção; no entanto, esses itens de auditoria serão retornados se **Mostrar resultados de todas as atividades** estiver selecionado.
   - **Usuários**: aceite o valor padrão em branco para retornar resultados para todos os usuários, ou insira um ou mais usuários.

3. Ao concluir, clique em **Pesquisar**. As atividades aparecem na nova página **Pesquisa de auditoria**.

4. Nos resultados, clique em **Filtrar resultados** e digite **Set-Mailbox** na caixa de filtro de atividade.

5. Selecione um registro de auditoria nos resultados para abrir o flyout **Details.**

Para obter mais informações, consulte [Pesquisar o log de auditoria para investigar problemas comuns de suporte.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)

---
title: Ler os logs de auditoria para eventos excluídos
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896003"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Ler os logs de auditoria para eventos excluídos

Veja como fazer isso:

1. Faça uma das seguintes ações:
   - Na Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para **Auditoria de** \> **Soluções.** Ou, para ir diretamente para a página **Auditoria,** use <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender em <https://security.microsoft.com> , vá para **Auditoria**. Ou, para ir diretamente para a página **Auditoria,** use <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Se você vir um aviso de que precisa ativar o recurso, vá em frente e a ligue agora. Se o recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.

2. Na guia **Pesquisa** da página **Auditoria,** configure as seguintes configurações:
   - **Intervalo de data e hora**: Selecione o intervalo de data/hora nas caixas **Iniciar** **e** Fim.
   - **Atividades**: insira **Exchange de caixa de** correio e selecione os seguintes valores:
     - **Mensagens excluídas da pasta Itens Excluídos**
     - **Mensagens movidas para a pasta Itens Excluídos**

       Quando terminar, clique fora do painel para minimizar o painel **Atividades.**

   - **Usuários**: Aceite o valor padrão em branco para retornar resultados para todos os usuários ou insira um ou mais usuários.

3. Quando terminar, clique em **Pesquisar**. As atividades aparecem na nova página **de pesquisa auditoria.**

4. Selecione uma atividade nos resultados para abrir o sobremenu de detalhes. Informações adicionais sobre o item excluído, como a linha de assunto e o local do item quando ele foi excluído, são exibidas no campo **AffectedItems.**

   > [!NOTE]
   > Não é possível restaurar itens excluídos usando o recurso de log de auditoria. Para restaurar itens excluídos, consulte [Recover deleted email messages in Outlook na Web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Para obter mais informações, consulte [Pesquisar o log de auditoria para investigar problemas comuns de suporte.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)

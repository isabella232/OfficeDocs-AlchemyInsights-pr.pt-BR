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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967321"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Ler os logs de auditoria para eventos excluídos

Veja como fazer isso:

1. Vá para o centro de conformidade [Office 365 segurança & segurança.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione **Pesquisa de** log de auditoria de  >  [**pesquisa**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Se você vir um aviso de que precisa ativar o recurso, vá em frente e a ligue agora. Se o recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.
1. Selecione **Atividades** e, em seguida, **encontre Exchange de caixa de correio**. Selecione as **mensagens excluídas da pasta Itens Excluídos** e As mensagens **movidas para as opções de** pasta Itens Excluídos. Quando terminar, clique fora do painel para minimizar o painel **Atividades.**
1. Especifique o intervalo de datas e, na caixa **Usuários,** selecione o nome de usuário do usuário que você deseja investigar. Você pode selecionar mais de um usuário por vez.
1. Selecione **Pesquisar**. As atividades são exibidas em **Resultados**.
1. Para exibir os detalhes, selecione uma atividade e selecione **Mais Informações.** Informações adicionais sobre o item excluído, como a linha de assunto e o local do item quando ele foi excluído, são exibidas no campo **AffectedItems.**
    > [!NOTE]
    > Não é possível restaurar itens excluídos usando o recurso de log de auditoria. Para restaurar itens excluídos, consulte [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).

Para saber mais, confira [Pesquisar o log Office 365 de auditoria para solucionar problemas de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)

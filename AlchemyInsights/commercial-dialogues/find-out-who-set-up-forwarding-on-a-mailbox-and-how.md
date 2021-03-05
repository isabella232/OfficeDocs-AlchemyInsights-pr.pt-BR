---
title: Descubra quem configurar o encaminhamento em uma caixa de correio e como
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464312"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Descubra quem configurar o encaminhamento em uma caixa de correio e como

Se o encaminhamento externo foi definido em uma caixa de correio, a atividade é auditada como parte do cmdlet Set-Mailbox. Veja como encontrar a atividade no log de auditoria:

1. Vá para o Centro de Conformidade e Segurança [& do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione **Pesquisa de** log de auditoria de >  **pesquisa**.
    > [!NOTE]
    > Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.
1. Certifique-se de **que o** campo Atividades está definido como Mostrar resultados para todas **as atividades** (o padrão). Especifique o intervalo de datas. Não é necessário especificar um nome de usuário.
1. Selecione **Pesquisar**. As atividades aparecem em **Resultados**.
1. Selecione **Resultados do Filtro** e insira **Set-mailbox** no campo **Filtro** atividade. Isso retorna todas **as atividades Set-Mailbox.**
1. Para exibir os detalhes, selecione uma atividade e selecione **Mais Informações.** Em **Parâmetros,** você pode ver o endereço de email de encaminhamento que foi definido na caixa de correio. O **UserID** representa o usuário que configura o encaminhamento externo na caixa de correio.
Para saber mais, confira Pesquisar o log de auditoria do [Office 365 para solucionar problemas de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)
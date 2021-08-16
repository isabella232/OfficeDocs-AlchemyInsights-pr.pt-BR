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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988167"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Descubra quem configurar o encaminhamento em uma caixa de correio e como

Se o encaminhamento externo foi definido em uma caixa de correio, a atividade é auditada como parte do cmdlet Set-Mailbox. Veja como encontrar a atividade no log de auditoria:

1. Vá para o centro de conformidade [Office 365 segurança & segurança.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione **Pesquisa de** log de auditoria de >  **pesquisa**.
    > [!NOTE]
    > Se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.
1. Certifique-se de **que o** campo Atividades está definido como Mostrar resultados para todas **as atividades** (o padrão). Especifique o intervalo de datas. Não é necessário especificar um nome de usuário.
1. Selecione **Pesquisar**. As atividades são exibidas em **Resultados**.
1. Selecione **Resultados do Filtro** e insira **Set-mailbox** no campo **Filtro** atividade. Isso retorna todas **as atividades Set-Mailbox.**
1. Para exibir os detalhes, selecione uma atividade e selecione **Mais Informações.** Em **Parâmetros,** você pode ver o endereço de email de encaminhamento que foi definido na caixa de correio. O **UserID** representa o usuário que configura o encaminhamento externo na caixa de correio.
Para saber mais, confira [Pesquisar o log Office 365 de auditoria para solucionar problemas de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)
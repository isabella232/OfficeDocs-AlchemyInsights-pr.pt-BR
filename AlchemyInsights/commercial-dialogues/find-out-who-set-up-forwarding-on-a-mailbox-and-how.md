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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317796"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Descubra quem configurar o encaminhamento em uma caixa de correio e como

Se o encaminhamento externo foi definido em uma caixa de correio, a atividade será auditada como parte do cmdlet **Set-Mailbox.** Veja como encontrar a atividade no log de auditoria:

1. Faça uma das seguintes ações:
   - No Centro de conformidade do Microsoft 365 em <https://compliance.microsoft.com>, vá para **Soluções** \> **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://compliance.microsoft.com/auditlogsearch>.
   - No portal do Microsoft 365 Defender em <https://security.microsoft.com>, vá para **Auditoria**. Ou para ir direto para a página **Auditoria**, use <https://security.microsoft.com/auditlogsearch>.

   **Observação**: se você vir um aviso de que precisa ativar a auditoria, vá em frente e a a ligue agora. Se esse recurso não estiver ligado, os resultados da pesquisa não poderão puxar dados de datas anteriores.

2. Na página **Auditoria**, verifique se a guia **Pesquisa** está selecionada e defina as seguintes configurações:
   - Selecione o intervalo de data/hora nas caixas **Iniciar** **e** Fim.
   - Verifique se **a caixa Atividades** contém Mostrar resultados de todas as **atividades**.

3. Ao concluir, clique em **Pesquisar**. As atividades aparecem na nova página **Pesquisa de auditoria**.

4. Nos resultados, clique na coluna **Atividade** para classificar os resultados e procure entradas **Set-Mailbox.**

5. Selecione uma atividade nos resultados para abrir o sobremenu de detalhes. Você precisa ver os detalhes de cada registro de auditoria para determinar se a atividade está relacionada ao encaminhamento de email:
   - **ObjectId**: o valor de alias da caixa de correio que foi modificada.
   - **Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de email de destino.
   - **UserId**: o usuário que configurou o encaminhamento de email na caixa de correio no **campo ObjectId.**

Para obter mais informações, [consulte Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).

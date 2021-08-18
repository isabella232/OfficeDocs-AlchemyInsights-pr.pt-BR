---
title: Identificar excluir eventos de mensagem em logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317582"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Logs de auditoria para mensagens de email excluídas

A partir de janeiro de 2019, a Microsoft está a ligar o log de auditoria de caixa de correio por padrão. Caso contrário, para revisar a exclusão de eventos de mensagem para um usuário específico, você precisa habilitar manualmente as ações de exclusão para auditoria. Se o log de auditoria de caixa de correio já estiver habilitado para sua organização ou para o usuário específico, siga as etapas abaixo.

1. Faça logoff no [Microsoft 365 de Conformidade](https://protection.office.com/)

2. Clique **em Pesquisa e Investigação** e selecione Pesquisa de Log de **Auditoria.**

3. Selecione o intervalo de datas nos campos **Data de** início e **Data de** término. Especifique o nome de usuário para o usuário que você deseja investigar (o usuário que excluiu os itens). No campo **Atividades,** selecione **Mensagens excluídas da** pasta Itens Excluídos e Mensagens movidas **para a pasta Itens Excluídos.**

4. Clique em **Pesquisar**.

Nos resultados, selecione um registro de auditoria. No sobremenu de detalhes, clique **em Mais Informações.** Informações adicionais sobre o item excluído (por exemplo, a linha de assunto e o local do item quando ele foi excluído) são exibidas no campo **AffectedItems.** A **propriedade ClientInfoString** mostrará se a exclusão ocorreu em Outlook, Outlook na Web (anteriormente conhecido como Outlook Web App) ou em qualquer outro dispositivo.

Para obter mais informações, [consulte Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Observação**: não é possível recuperar itens excluídos usando o recurso de log de auditoria. Para recuperar mensagens excluídas no Outlook na Web, consulte [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).

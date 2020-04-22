---
title: Identificar eventos de mensagens de exclusão nos logs de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716484"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Logs de auditoria para mensagens de email excluídas

A partir de janeiro de 2019, a Microsoft está ativando o log de auditoria de caixa de correio por padrão. Caso contrário, para revisar excluir eventos de mensagem para um usuário específico, você precisará habilitar manualmente as ações de exclusão para auditoria. Se o log de auditoria de caixa de correio já estiver habilitado para sua organização ou para o usuário específico, siga as etapas abaixo.

1. Faça logon no [centro de conformidade & segurança da Microsoft 365](https://protection.office.com/)

2. Clique em **pesquisa e investigação** e selecione **pesquisa de log de auditoria**.

3. Selecione o intervalo de datas nos campos **data de início** e data de **término** . Especifique o nome de usuário para o usuário que você deseja investigar (o usuário que excluiu os itens). No campo **atividades** , selecione **mensagens excluídas da pasta itens excluídos** e **mensagens movidas para a pasta itens excluídos**.

4. Clique em **Pesquisar**.

Nos resultados, selecione um registro de auditoria. No submenu detalhes, clique em **mais informações**. Informações adicionais sobre o item excluído (por exemplo, a linha de assunto e o local do item quando ele foi excluído) são exibidas no campo **AffectedItems** . A propriedade **ClientInfoString** mostrará se a exclusão ocorreu no Outlook, no Outlook na Web (anteriormente conhecido como Outlook Web App) ou em qualquer outro dispositivo.

Para obter mais informações, consulte [determinando quem configurou o encaminhamento de email para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Observação**: não é possível recuperar itens excluídos usando o recurso de log de auditoria. Para recuperar mensagens excluídas no Outlook na Web, confira [recuperar itens excluídos no Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).

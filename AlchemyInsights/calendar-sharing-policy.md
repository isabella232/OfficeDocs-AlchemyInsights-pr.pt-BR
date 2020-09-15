---
title: 618 política de compartilhamento de calendário
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684218"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Erro de política ao compartilhar um calendário

1. Execute um dos seguintes procedimentos, conforme apropriado para sua situação:
    - Conecte-se ao Exchange Online usando o PowerShell remoto. Para obter mais informações, consulte [conectar-se ao Exchange Online usando o PowerShell remoto](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - No servidor local, abra o Shell de gerenciamento do Exchange.
2. Determine a política de compartilhamento que é atribuída ao usuário. Para fazer isso, execute o seguinte comando e anote a política retornada:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atualize a política de compartilhamento para o usuário. Para fazer isso, siga estas etapas:
    - Abra o centro de administração do Exchange.
    - Clique em **organização**e, em seguida, clique duas vezes na política atribuída ao usuário em **compartilhamento individual**. Esta é a política retornada na etapa 2.
    - Na página regra de compartilhamento, selecione o nível de compartilhamento de calendário que você deseja permitir em **especifique quais informações você deseja compartilhar**; clique em **salvar**.

Para obter mais informações, consulte: ["a política não permite conceder permissões neste nível a um ou mais dos destinatários" quando o usuário tenta compartilhar o calendário](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).

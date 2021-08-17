---
title: Política de compartilhamento de calendários 618
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091577"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Erro de política ao compartilhar um calendário

1. Faça um dos seguintes procedimentos, conforme apropriado para sua situação:
    - Conexão para Exchange Online usando o PowerShell Remoto. Para obter mais informações, [consulte Conexão Exchange Online usando o Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - No servidor local, abra o Shell Exchange Gerenciamento.
2. Determine a política de compartilhamento atribuída ao usuário. Para fazer isso, execute o seguinte comando e observe a política retornada:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atualize a política de compartilhamento para o usuário. Para fazer isso, execute estas etapas:
    - Abra o centro de administração do Exchange.
    - Clique **em** Organização e clique duas vezes na política atribuída ao usuário em **Compartilhamento Individual.** Esta é a política retornada na etapa 2.
    - Na página Regra de Compartilhamento, selecione o nível de compartilhamento de calendário que você deseja permitir em **Especificar quais informações você deseja compartilhar;** clique **em Salvar**.

Para obter mais informações, consulte: "A política não permite conceder permissões nesse nível a um ou mais dos [destinatários",](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)quando o usuário tentar compartilhar calendário .

---
title: Corrigir problemas de entrega de emails em pastas públicas habilitadas para email
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401316"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Corrigir problemas de entrega de emails em pastas públicas habilitadas para email

Se os remetentes externos não podem enviar mensagens para suas pastas públicas habilitadas para email, e os remetentes receberem o erro: **não foi possível encontrar (550 5.4.1)**, verifique se o domínio de email da pasta pública está configurado como um domínio de retransmissão interno em vez de um domínio autoritativo:

1. Abra o [centro de administração do Exchange (Eat)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Vá para **** \> **domínios aceitos**do fluxo de emails, selecione o domínio aceito e clique em **Editar**.

3. Na página de propriedades que será aberta, se o tipo de domínio estiver definido como **autoritativo**, altere o valor para **retransmissão interna** e clique em **salvar**.

Se os remetentes externos receberem o erro **que você não tem permissão (550 5.7.13)**, execute o seguinte comando no [PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para usuários anônimos na pasta pública:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Para permitir que usuários externos enviem email para esta pasta pública, adicione o direito de acesso createItems ao usuário anônimo. Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.

---
title: Corrigir problemas de entrega de email para pastas públicas habilitadas para email
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
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068800"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Corrigir problemas de entrega de email para pastas públicas habilitadas para email

Se os envios externos não puderem enviar mensagens para suas pastas públicas habilitadas para email e os enviadores receberem o erro: não foi possível encontrar **(550 5.4.1),** verifique se o domínio de email para a pasta pública está configurado como um domínio de retransmissão interno em vez de um domínio autoritativo:

1. Abra o [Exchange de administração (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Vá para **Fluxo de email** \> **Domínios aceitos,** selecione o domínio aceito e clique em **Editar**.

3. Na página propriedades que será aberta, se o tipo de domínio  estiver definido como **Autoritativo,** altere o valor para Retransmissão Interna e clique em **Salvar**.

Se os envios externos receberem o erro, você não terá permissão **(550 5.7.13),** execute o seguinte comando no [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para usuários anônimos na pasta pública:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Para permitir que usuários externos enviem emails para essa pasta pública, adicione o acesso CreateItems direito ao usuário Anônimo. Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.

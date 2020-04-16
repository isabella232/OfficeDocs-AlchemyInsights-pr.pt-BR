---
title: Configurar respostas automáticas para uma caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509476"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Configurar respostas automáticas para uma caixa de correio de um usuário

**Método 1**

1. Entre no portal do Office 365.

2. Vá para **Usuários > Usuários ativos** (ou **Grupos > Caixas de correio compartilhadas** se você definir essa opção em uma caixa de correio compartilhada).

3. Selecione um usuário com uma caixa de correio do Microsoft Exchange.

4. No menu do submenu à direita, vá para **Configurações de email > Respostas automáticas** (se for uma caixa de correio compartilhada, basta clicar **Respostas automáticas**no menu do submenu).

**Método 2**

1. Entre no portal de administração do Office 365 usando as credenciais de administrador.

2. Escolha **Centros de Administração** e depois clique em **Exchange**. 

3. Clique na imagem no canto superior direito, clique **Outro usuário** e, em seguida, selecione a caixa de correio de usuário que você deseja alterar.

4. No lado esquerdo, selecione **Opções**, clique em **Organizar email** e, em seguida, clique em **Respostas automáticas.**

**Método 3**

Execute os seguintes cmdlet no PowerShell do Exchange Online:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Para obter mais informações sobre esse cmdlet, confira [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
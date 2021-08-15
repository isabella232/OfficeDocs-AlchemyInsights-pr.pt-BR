---
title: Lembrar ou substituir uma mensagem de email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024374"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Recall or replace an email message in Microsoft 365

- Você só **pode lembrar mensagens enviadas para pessoas em sua organização.** Por exemplo, se a mensagem foi enviada para um endereço do Gmail, você não poderá relembá-la.
- Você só **pode lembrar mensagens enviadas de Outlook para o computador**. Se um usuário enviar uma mensagem usando Outlook para Mac ou Outlook na Web, você não poderá relembra-la.
- Como administrador de locatários, você pode lembrar mensagens em nome dos usuários usando o **PowerShell** (Para obter mais informações, consulte: Pesquisar e [excluir mensagens de email](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Não é possível lembrar mensagens do centro de administração. Role para baixo para "Pesquisar e excluir mensagens de email em sua organização" para obter mais informações.

**Recall or replace an email message that you sent**

1. No painel de pastas à esquerda da janela Outlook, escolha a pasta Itens Enviados.
2. Abra a mensagem que você deseja lembrar. Clique duas vezes para abrir a mensagem. Selecionar a mensagem para que ela apareça no painel de leitura não permitirá que você relembre a mensagem.
3. Na guia Mensagem, selecione **Ações**  >  **Recall This Message**.
4. Escolha **Excluir cópias não lidas dessa** mensagem ou Excluir cópias não **lidas** e substitua por uma nova mensagem e selecione **OK**.
5. Se você estiver enviando uma mensagem de substituição, recomponha a mensagem e selecione **Enviar**.
6. O sucesso ou falha de um recall de mensagem depende das configurações dos destinatários Outlook.

Para obter mais informações, incluindo como verificar o recall, consulte [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Para pesquisar e excluir mensagens de email em sua*** organização, é mais fácil se você for um administrador global. Se você não for um administrador global, sua conta deverá ser adicionada ao grupo de funções do Gerenciador de Descobertas e, ou à função de gerenciamento de Pesquisa de Conformidade. Para excluir mensagens, você precisará ingressar no grupo de função Gerenciamento da Organização ou na função de gerenciamento de Pesquisa e Limpeza. As permissões para essas funções são atribuídas no centro de conformidade & [segurança.](https://protection.office.com/)

1. [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/content-search) para encontrar a mensagem a ser excluído.
2. [Conectar-se ao PowerShell do Centro de Conformidade e Segurança](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Se você estiver usando o MFA (autenticação multifatória), consulte Conexão para Microsoft 365 & Centro de Conformidade e Segurança do PowerShell usando a autenticação [multifatória](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).

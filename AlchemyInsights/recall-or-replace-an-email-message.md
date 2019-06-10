---
title: Cancelar ou substituir uma mensagem de email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 461969bee3b871fd2c4a8418406ea2b6de791191
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770797"
---
# <a name="recall-or-replace-an-email-message"></a>Cancelar ou substituir uma mensagem de email

- Você **só pode recuperar mensagens que são enviadas para pessoas em sua organização**. Se a mensagem foi enviada para um endereço do Gmail, por exemplo, não é possível recuperá-la.
- Você pode **apenas recuperar mensagens enviadas do Outlook 2016 para o PC**. Se um usuário enviar uma mensagem usando o Outlook para Mac ou o Outlook na Web, você não poderá recuperá-la.
- Se você for um administrador, poderá **recuperar mensagens em nome dos usuários usando o PowerShell**. Não é possível recuperar mensagens do centro de administração. Role para baixo até "procurar e excluir mensagens de email em sua organização" para obter mais informações.

***Cancelar ou substituir uma mensagem de email enviada***
1. No painel de pastas à esquerda da janela do Outlook, escolha a pasta Itens enviados.
2. Abra a mensagem que você deseja cancelar. Você deve clicar duas vezes para abrir a mensagem. Selecionar a mensagem para que ela apareça no painel de leitura não permite que você relembre a mensagem.
3. Na guia mensagem, selecione **ações** > **cancelar esta mensagem**.
4. Escolha **Excluir cópias não lidas desta mensagem** ou **Excluir cópias não lidas e substituir por uma nova mensagem**e, em seguida, selecione **OK**.
5. Se você estiver enviando uma mensagem de substituição, redija a mensagem e selecione **Enviar**.
6. O sucesso ou a falha de uma recuperação de mensagem depende das configurações dos destinatários no Outlook. 

Para obter mais informações, incluindo como verificar o cancelamento, confira [cancelar ou substituir uma mensagem de email enviada](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Procurar e excluir mensagens de email em sua organização*** Para pesquisar e excluir mensagens de email em sua organização, é mais fácil se você for um administrador global. Se você não for um administrador global, sua conta deverá ser adicionada ao grupo de funções Gerenciador de descoberta eletrônica ou à função de gerenciamento de pesquisa de conformidade. Para excluir mensagens, você precisará ingressar no grupo de função gerenciamento da organização ou na função gerenciamento de pesquisa e limpeza. As permissões para essas funções são atribuídas no [centro de conformidade de & de segurança](https://protection.office.com/).

1. [Criar uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para localizar a mensagem a ser excluída.
2. [Conecte-se ao PowerShell do centro de conformidade & segurança](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Se você estiver usando a MFA, confira [conectar-se ao PowerShell do centro de conformidade & segurança do Office 365 usando a autenticação](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)multifator. 
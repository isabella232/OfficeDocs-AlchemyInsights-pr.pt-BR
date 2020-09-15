---
title: Cancelar a área de trabalho do Outlook ou substituir uma mensagem de email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663978"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Cancelar ou substituir uma mensagem de email do Outlook

- Como administrador, você pode **recuperar mensagens em nome de usuários usando o PowerShell**. Não é possível recuperar mensagens do centro de administração.
- Você **só pode recuperar mensagens que são enviadas para pessoas em sua organização**. Se a mensagem foi enviada para um endereço do Gmail, por exemplo, não é possível recuperá-la.
- Você **só pode recuperar mensagens enviadas do Outlook 2016 no computador**. Se um usuário enviar uma mensagem usando o Outlook para Mac ou o Outlook na Web, você não poderá recuperá-la.

Para cancelar ou substituir uma mensagem de email:

1. No painel de pastas à esquerda da janela do Outlook, selecione a pasta Itens enviados.
1. Clique duas vezes na mensagem que você deseja cancelar para abri-la.
1. Selecione a guia **mensagem** e, em seguida, selecione **ações**  >  **cancelar esta mensagem**.
1. Selecione **Excluir cópias não lidas desta mensagem** ou **Excluir cópias não lidas e substituir por uma nova mensagem**e, em seguida, selecione **OK**.
1. Se você estiver enviando uma mensagem de substituição, redija a mensagem e selecione **Enviar**.
1. O sucesso ou a falha de uma recuperação de mensagem depende das configurações do destinatário no Outlook. Para ver as etapas para verificar o cancelamento, confira [Este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Pesquisar e excluir mensagens de email em sua organização

- Se você não for um administrador global, sua conta deverá ser adicionada à função de gerente de descoberta eletrônica ou à função de gerenciamento de pesquisa de conformidade para pesquisar mensagens. Para excluir mensagens, você precisará ingressar no grupo de função gerenciamento da organização ou na função gerenciamento de pesquisa e limpeza. As permissões para essas funções são atribuídas no [centro de conformidade e segurança](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Criar uma pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/content-search) para localizar a mensagem a ser excluída.
- [Conecte-se ao PowerShell do centro de conformidade e segurança](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Se você estiver usando a autenticação multifator, confira [conectar-se ao PowerShell do centro de conformidade e segurança do Microsoft 365 usando a autenticação multifator](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).
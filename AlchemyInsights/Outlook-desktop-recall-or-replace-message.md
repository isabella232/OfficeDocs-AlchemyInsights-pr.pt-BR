---
title: Outlook Recall da área de trabalho ou substituir uma mensagem de email
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918383"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Recall or replace an Outlook email

- Como administrador, você pode lembrar mensagens **em nome de usuários que usam o PowerShell**. Não é possível lembrar mensagens do centro de administração.
- Você só **pode lembrar mensagens enviadas para pessoas em sua organização.** Se a mensagem foi enviada para um endereço do Gmail, por exemplo, você não poderá relembá-la.
- Você só **pode lembrar mensagens enviadas de Outlook 2016 no computador**. Se um usuário enviar uma mensagem usando Outlook para Mac ou Outlook na Web, você não poderá relembra-la.

Para lembrar ou substituir uma mensagem de email:

1. No painel de pastas à esquerda da janela Outlook, selecione a pasta Itens Enviados.
1. Clique duas vezes na mensagem que você deseja lembrar para abri-la.
1. Selecione a **guia Mensagem** e selecione **Ações** Recall  >  **This Message**.
1. Selecione **Excluir cópias não lidas dessa** mensagem ou Excluir cópias não **lidas** e substitua por uma nova mensagem e selecione **OK**.
1. Se você estiver enviando uma mensagem de substituição, recomponha a mensagem e selecione **Enviar**.
1. O sucesso ou falha de um recall de mensagem depende das configurações do destinatário em Outlook. Para ver as etapas para verificar o recall, consulte [este artigo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Pesquisar e excluir mensagens de email em sua organização

- Se você não for um administrador global, sua conta deverá ser adicionada à função de Gerenciador de Descobertas esdiscovery ou à função de gerenciamento de Pesquisa de Conformidade para pesquisar mensagens. Para excluir mensagens, você precisará ingressar no grupo de função Gerenciamento da Organização ou na função de gerenciamento de Pesquisa e Limpeza. As permissões para essas funções são atribuídas no centro [de segurança e conformidade.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/content-search) para encontrar a mensagem a ser excluído.
- [Conexão o PowerShell do Centro](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)de Conformidade e Segurança.

Se você estiver usando autenticação multifatória, consulte Conexão para Microsoft 365 segurança e o Centro de Conformidade [do PowerShell usando a autenticação multifatória](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).
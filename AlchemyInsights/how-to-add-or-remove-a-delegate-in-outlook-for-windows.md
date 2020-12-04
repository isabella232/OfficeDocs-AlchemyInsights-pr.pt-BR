---
title: Como adicionar ou remover um representante no Outlook para Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571769"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Como adicionar ou remover um representante no Outlook para Windows

Para adicionar um representante no Outlook para Windows: 

1. Clique na guia **arquivo** seguida por **configurações de conta** e escolha acesso de **Representante**.
2. Clique em **Adicionar**. Se **Add** não aparecer, uma conexão ativa pode não existir entre o Outlook e o Exchange. A barra de status do Outlook exibe o status da conexão.
3. Digite o nome da pessoa que você deseja designar como seu representante ou pesquise e escolha o nome na lista de resultados da pesquisa.

    > [!NOTE]
    > O representante deve ser uma pessoa na GAL (lista de endereços global) do Exchange da sua organização.
4. Clique em **Adicionar** seguido por **OK**.
5. Na caixa de diálogo **permissões de representante** , aceite as configurações de permissão padrão ou selecione níveis de acesso personalizados para pastas do Exchange.

    - Se um representante precisar de permissão para trabalhar apenas com solicitações de reunião e respostas, as configurações de permissão padrão, como **Representante, receberá cópias de mensagens relacionadas à reunião enviadas para mim** são suficientes. Você pode deixar a configuração de permissão de **caixa de entrada** como **nenhum**. As solicitações e respostas de reunião vão diretamente para a caixa de entrada do representante.

    > [!NOTE]
    > Por padrão, o representante tem a permissão **Editor (pode ler, criar e modificar itens)** na pasta **calendário** . Quando o representante responde a uma reunião em seu nome, ele é automaticamente adicionado à pasta **calendário** .

5. Para enviar uma mensagem para notificar o representante das permissões alteradas, marque a caixa de seleção **Enviar automaticamente uma mensagem para o representante Resumindo estas permissões** .
6. Se desejar, marque a caixa de seleção **Representante pode ver meus itens particulares** .

    > [!IMPORTANT]
    > Essa configuração afeta todas as pastas do Exchange. Isso inclui todos os emails, contatos, calendário, tarefas, anotações e pastas de diário. Não há como conceder acesso a itens privados em apenas pastas especificadas.

7. Escolha **OK**.

    > [!NOTE]
    >
    > - As mensagens enviadas com as permissões Enviar em nome de incluem o representante **de**. Quando uma mensagem é enviada com permissões Enviar como, apenas seu nome é exibido.
    > - Depois que você adicionar alguém como representante, poderá adicionar sua caixa de correio do Exchange ao seu perfil do Outlook. Para obter instruções, consulte [gerenciar itens de email e calendário de outra pessoa](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Para remover um representante no Outlook para Windows:

1. Clique na guia **arquivo** .
2. Clique em **configurações de conta** seguidas por **acesso de representante**.
3. Escolha o nome do representante para o qual você deseja alterar as permissões e clique em **remover** seguido por **OK**.

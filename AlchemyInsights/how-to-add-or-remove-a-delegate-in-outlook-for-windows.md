---
title: Como adicionar ou remover um Representante no Outlook para Windows
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
ms.openlocfilehash: ee54e2bcca4f4591b33ee805290192311f6cde09a9e453a813e9db328d19634d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945325"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Como adicionar ou remover um Representante no Outlook para Windows

Para adicionar um Representante no Outlook para Windows: 

1. Clique na guia **Arquivo** seguido por **Conta Configurações** e escolha **Delegar Acesso**.
2. Clique em **Adicionar**. Se **Add** não aparecer, uma conexão ativa pode não existir entre Outlook e Exchange. A Outlook de status exibe o status da conexão.
3. Digite o nome da pessoa que você deseja designar como representante ou pesquise e escolha o nome na lista de resultados da pesquisa.

    > [!NOTE]
    > O representante deve ser uma pessoa na Exchange gal (lista de endereços global) da sua organização.
4. Clique em **Adicionar** seguido por **OK**.
5. Na caixa **de diálogo Permissões** de Representante, aceite as configurações de permissão padrão ou selecione níveis de acesso personalizados para Exchange pastas.

    - Se um representante precisar de permissão para trabalhar somente com solicitações e respostas de reunião, as configurações de permissão padrão, como Delegate, receberão cópias de mensagens **relacionadas** à reunião enviadas a mim são suficientes. Você pode deixar a **configuração de permissão Caixa** de Entrada em **Nenhum**. As solicitações e respostas de reunião irão diretamente para a caixa de entrada do representante.

    > [!NOTE]
    > Por padrão, o representante tem permissão **editor (pode ler,** criar e modificar itens) para sua **pasta Calendário.** Quando o representante responde a uma reunião em seu nome, ela é automaticamente adicionada à **pasta Calendário.**

5. Para enviar uma mensagem para notificar o representante das permissões alteradas, marque a caixa de seleção Enviar automaticamente uma mensagem para delegar resumindo **essas** permissões.
6. Se quiser, selecione a caixa de seleção **Delegar pode ver meus itens** particulares.

    > [!IMPORTANT]
    > Essa configuração afeta todas as Exchange pastas. Isso inclui todas as pastas Mail, Contacts, Calendar, Tasks, Notes e Journal. Não há como conceder acesso a itens particulares apenas em pastas especificadas.

7. Escolha **OK**.

    > [!NOTE]
    >
    > - As mensagens enviadas com permissões Enviar em Nome incluem os nomes do representante e seus ao lado de **From**. Quando uma mensagem é enviada com permissões Enviar como, apenas seu nome é exibido.
    > - Depois de adicionar alguém como representante, ele poderá adicionar sua caixa de correio Exchange seu perfil Outlook pessoal. Para obter instruções, [consulte Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Para remover um Representante no Outlook para Windows:

1. Clique na guia **Arquivo.**
2. Clique em **Conta Configurações** seguido por **Delegate Access**.
3. Escolha o nome do representante para o qual você deseja alterar as permissões e clique em **Remover** seguido por **OK**.

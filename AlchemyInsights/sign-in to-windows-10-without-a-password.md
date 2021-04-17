---
title: Entrar no Windows 10 sem usar uma senha
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830534"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Entrar no Windows 10 sem usar uma senha

Para evitar precisar digitar uma senha na inicialização do Windows, recomendamos usar uma das opções de login seguro do Windows Hello, como PIN, reconhecimento de rosto ou impressão digital, se disponível. Se você realmente quiser desabilitar a conexão segura, consulte as instruções "Entrar automaticamente no Windows 10" abaixo.

**Proteger alternativas do Windows Hello para a senha da conta**

Vá para **Configurações > Contas > opções de** login (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)). As opções de login disponíveis serão listadas. Por exemplo:

![Opções de login.](media/sign-in-options.png)

Clique ou toque em uma das opções para configurá-la. Na próxima vez que você iniciar ou desbloquear o Windows, poderá usar a nova opção em vez de uma senha. 

**Entrar automaticamente no Windows 10**

**Observação**: a assinatura automática é conveniente, mas apresenta um risco de segurança, especialmente se o computador estiver acessível por várias pessoas. 

1. Clique ou toque no **botão Iniciar** na Barra de Tarefas.

2. Digite **netplwiz** e a tecla Enter para abrir a janela Contas de Usuário.

3. Em **Contas de Usuário,** clique na conta na que você deseja entrar automaticamente quando o Windows for iniciado.

4. Desmarque a caixa de seleção "Os usuários devem inserir um nome de usuário e uma senha para usar este computador".

    ![Os usuários devem inserir uma opção de nome de usuário e senha.](media/users-must-enter-username.png)

5. Clique em **OK**. Você será solicitado a inserir e confirmar a senha da conta selecionada. Clique em **OK** para concluir. Na próxima vez que o Windows 10 for iniciado, ele entrará automaticamente na conta selecionada.

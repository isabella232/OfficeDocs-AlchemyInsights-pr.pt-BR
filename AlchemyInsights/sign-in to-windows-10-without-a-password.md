---
title: Entrar no Windows 10 sem usar uma senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588269"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Entrar no Windows 10 sem usar uma senha

Para evitar ter que digitar uma senha na inicialização do Windows, recomendamos que você use uma das opções de entrada segura do Windows Hello, como um PIN, um reconhecimento de face ou impressão digital, se disponível. Se você quiser desabilitar a entrada segura, consulte as instruções "entrar automaticamente no Windows 10" abaixo.

**Proteger as alternativas do Windows Hello para a senha da conta**

Vá até **configurações > contas > opções de entrada** (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)). As opções de entrada disponíveis serão listadas. Por exemplo:

![Opções de entrada.](media/sign-in-options.png)

Clique ou toque em uma das opções para configurá-la. Na próxima vez que iniciar ou desbloquear o Windows, você poderá usar a nova opção em vez de uma senha. 

**Entrar automaticamente no Windows 10**

**Observação**: a entrada automática é conveniente, mas apresenta um risco de segurança, especialmente se o seu computador estiver acessível por várias pessoas. 

1. Clique ou toque no botão **Iniciar** na barra de tarefas.

2. Digite **netplwiz** e pressione a tecla Enter para abrir a janela contas de usuário.

3. Em **contas de usuário**, clique na conta na qual você deseja entrar automaticamente quando o Windows for iniciado.

4. Desmarque a caixa de seleção "os usuários devem digitar um nome de usuário e senha para usar este computador".

    ![Os usuários devem inserir uma opção de nome de usuário e senha.](media/users-must-enter-username.png)

5. Clique em **OK**. Você será solicitado a inserir e confirmar a senha para a conta que você selecionou. Clique em **OK** para concluir. Na próxima vez que o Windows 10 for iniciado, ele entrará automaticamente na conta que você selecionou.

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
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107492"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Entrar no Windows 10 sem usar uma senha

Para evitar ter que digitar uma senha na inicialização Windows, recomendamos que você use uma das opções de Windows Hello de login seguro, como PIN, reconhecimento de rosto ou impressão digital, se disponível. Se você realmente deseja desabilitar a conexão segura, consulte as instruções "Entrar automaticamente Windows 10" abaixo.

**Proteger Windows Hello alternativas à senha da conta**

Vá para **Configurações > contas > opções de login** (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)). As opções de login disponíveis serão listadas. Por exemplo:

![Opções de login.](media/sign-in-options.png)

Clique ou toque em uma das opções para configurá-la. Na próxima vez que você iniciar ou desbloquear Windows, você poderá usar a nova opção em vez de uma senha. 

**Entrar automaticamente no Windows 10**

**Observação**: a assinatura automática é conveniente, mas apresenta um risco de segurança, especialmente se o computador estiver acessível por várias pessoas. 

1. Clique ou toque no **botão Iniciar** na Barra de Tarefas.

2. Digite **netplwiz** e a tecla Enter para abrir a janela Contas de Usuário.

3. Em **Contas de Usuário,** clique na conta na que você deseja entrar automaticamente quando Windows iniciar.

4. Desmarque a caixa de seleção "Os usuários devem inserir um nome de usuário e uma senha para usar este computador".

    ![Os usuários devem inserir uma opção de nome de usuário e senha.](media/users-must-enter-username.png)

5. Clique em **OK**. Você será solicitado a inserir e confirmar a senha da conta selecionada. Clique em **OK** para concluir. Na próxima Windows 10, ele entrará automaticamente na conta selecionada.

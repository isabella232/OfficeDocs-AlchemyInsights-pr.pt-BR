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
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="d7b3f-102">Entrar no Windows 10 sem usar uma senha</span><span class="sxs-lookup"><span data-stu-id="d7b3f-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="d7b3f-103">Para evitar precisar digitar uma senha na inicialização do Windows, recomendamos usar uma das opções de login seguro do Windows Hello, como PIN, reconhecimento de rosto ou impressão digital, se disponível.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="d7b3f-104">Se você realmente quiser desabilitar a conexão segura, consulte as instruções "Entrar automaticamente no Windows 10" abaixo.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="d7b3f-105">**Proteger alternativas do Windows Hello para a senha da conta**</span><span class="sxs-lookup"><span data-stu-id="d7b3f-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="d7b3f-106">Vá para **Configurações > Contas > opções de** login (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="d7b3f-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d7b3f-107">As opções de login disponíveis serão listadas.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="d7b3f-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="d7b3f-108">For example:</span></span>

![Opções de login.](media/sign-in-options.png)

<span data-ttu-id="d7b3f-110">Clique ou toque em uma das opções para configurá-la.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="d7b3f-111">Na próxima vez que você iniciar ou desbloquear o Windows, poderá usar a nova opção em vez de uma senha.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="d7b3f-112">**Entrar automaticamente no Windows 10**</span><span class="sxs-lookup"><span data-stu-id="d7b3f-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="d7b3f-113">**Observação**: a assinatura automática é conveniente, mas apresenta um risco de segurança, especialmente se o computador estiver acessível por várias pessoas.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="d7b3f-114">Clique ou toque no **botão Iniciar** na Barra de Tarefas.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="d7b3f-115">Digite **netplwiz** e a tecla Enter para abrir a janela Contas de Usuário.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="d7b3f-116">Em **Contas de Usuário,** clique na conta na que você deseja entrar automaticamente quando o Windows for iniciado.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="d7b3f-117">Desmarque a caixa de seleção "Os usuários devem inserir um nome de usuário e uma senha para usar este computador".</span><span class="sxs-lookup"><span data-stu-id="d7b3f-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Os usuários devem inserir uma opção de nome de usuário e senha.](media/users-must-enter-username.png)

5. <span data-ttu-id="d7b3f-119">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-119">Click **OK**.</span></span> <span data-ttu-id="d7b3f-120">Você será solicitado a inserir e confirmar a senha da conta selecionada.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="d7b3f-121">Clique em **OK** para concluir.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-121">Click **OK** to finish.</span></span> <span data-ttu-id="d7b3f-122">Na próxima vez que o Windows 10 for iniciado, ele entrará automaticamente na conta selecionada.</span><span class="sxs-lookup"><span data-stu-id="d7b3f-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>

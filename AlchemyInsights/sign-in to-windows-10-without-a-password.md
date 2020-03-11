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
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="24d3b-102">Entrar no Windows 10 sem usar uma senha</span><span class="sxs-lookup"><span data-stu-id="24d3b-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="24d3b-103">Para evitar ter que digitar uma senha na inicialização do Windows, recomendamos que você use uma das opções de entrada segura do Windows Hello, como um PIN, um reconhecimento de face ou impressão digital, se disponível.</span><span class="sxs-lookup"><span data-stu-id="24d3b-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="24d3b-104">Se você quiser desabilitar a entrada segura, consulte as instruções "entrar automaticamente no Windows 10" abaixo.</span><span class="sxs-lookup"><span data-stu-id="24d3b-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="24d3b-105">**Proteger as alternativas do Windows Hello para a senha da conta**</span><span class="sxs-lookup"><span data-stu-id="24d3b-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="24d3b-106">Vá até **configurações > contas > opções de entrada** (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="24d3b-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="24d3b-107">As opções de entrada disponíveis serão listadas.</span><span class="sxs-lookup"><span data-stu-id="24d3b-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="24d3b-108">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="24d3b-108">For example:</span></span>

![Opções de entrada.](media/sign-in-options.png)

<span data-ttu-id="24d3b-110">Clique ou toque em uma das opções para configurá-la.</span><span class="sxs-lookup"><span data-stu-id="24d3b-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="24d3b-111">Na próxima vez que iniciar ou desbloquear o Windows, você poderá usar a nova opção em vez de uma senha.</span><span class="sxs-lookup"><span data-stu-id="24d3b-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="24d3b-112">**Entrar automaticamente no Windows 10**</span><span class="sxs-lookup"><span data-stu-id="24d3b-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="24d3b-113">**Observação**: a entrada automática é conveniente, mas apresenta um risco de segurança, especialmente se o seu computador estiver acessível por várias pessoas.</span><span class="sxs-lookup"><span data-stu-id="24d3b-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="24d3b-114">Clique ou toque no botão **Iniciar** na barra de tarefas.</span><span class="sxs-lookup"><span data-stu-id="24d3b-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="24d3b-115">Digite **netplwiz** e pressione a tecla Enter para abrir a janela contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="24d3b-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="24d3b-116">Em **contas de usuário**, clique na conta na qual você deseja entrar automaticamente quando o Windows for iniciado.</span><span class="sxs-lookup"><span data-stu-id="24d3b-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="24d3b-117">Desmarque a caixa de seleção "os usuários devem digitar um nome de usuário e senha para usar este computador".</span><span class="sxs-lookup"><span data-stu-id="24d3b-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Os usuários devem inserir uma opção de nome de usuário e senha.](media/users-must-enter-username.png)

5. <span data-ttu-id="24d3b-119">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="24d3b-119">Click **OK**.</span></span> <span data-ttu-id="24d3b-120">Você será solicitado a inserir e confirmar a senha para a conta que você selecionou.</span><span class="sxs-lookup"><span data-stu-id="24d3b-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="24d3b-121">Clique em **OK** para concluir.</span><span class="sxs-lookup"><span data-stu-id="24d3b-121">Click **OK** to finish.</span></span> <span data-ttu-id="24d3b-122">Na próxima vez que o Windows 10 for iniciado, ele entrará automaticamente na conta que você selecionou.</span><span class="sxs-lookup"><span data-stu-id="24d3b-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>

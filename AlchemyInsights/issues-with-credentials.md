---
title: Problemas com credenciais
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052941"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="26d8e-102">Problemas com credenciais</span><span class="sxs-lookup"><span data-stu-id="26d8e-102">Issues with credentials</span></span>

<span data-ttu-id="26d8e-103">[A microsoft identity platform and the OAuth 2.0 client credentials flow describes](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) how to program directly against the OAuth 2.0 client credentials grant flow.</span><span class="sxs-lookup"><span data-stu-id="26d8e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="26d8e-104">**Como faço para gerenciar a senha ou as credenciais de certificado de um aplicativo?**</span><span class="sxs-lookup"><span data-stu-id="26d8e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="26d8e-105">Na CLI do Azure, você pode usar a credencial do aplicativo [az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) para excluir, listar ou redefinir as credenciais de senha ou certificado de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26d8e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="26d8e-106">**Como meus usuários redefinem suas senhas?**</span><span class="sxs-lookup"><span data-stu-id="26d8e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="26d8e-107">Os usuários precisam [se registrar para redefinir senhas](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) de autoatendados antes de redefinir suas senhas.</span><span class="sxs-lookup"><span data-stu-id="26d8e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="26d8e-108">Depois que um usuário se registrar, ele poderá seguir as instruções neste artigo para redefinir sua senha: [redefinir sua senha de](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)trabalho ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="26d8e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="26d8e-109">**Como meus usuários alteram suas senhas?**</span><span class="sxs-lookup"><span data-stu-id="26d8e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="26d8e-110">Os usuários podem seguir as etapas deste artigo para alterar suas senhas: [Como alterar sua senha.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="26d8e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="26d8e-111">Eles também podem [gerenciar senhas de aplicativo para verificação em duas etapas.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="26d8e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="26d8e-112">**Meu usuário está recebendo um erro ao alterar ou redefinir a senha**</span><span class="sxs-lookup"><span data-stu-id="26d8e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="26d8e-113">Este link fornecerá informações sobre problemas comuns que podem surgir quando um usuário está tentando redefinir sua senha: problemas [comuns e suas soluções](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="26d8e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="26d8e-114">**Estou com um problema para redefinir a senha de um usuário**</span><span class="sxs-lookup"><span data-stu-id="26d8e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="26d8e-115">Certifique-se de que você está autorizado a redefinir senhas.</span><span class="sxs-lookup"><span data-stu-id="26d8e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="26d8e-116">*Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.*</span><span class="sxs-lookup"><span data-stu-id="26d8e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="26d8e-117">Os administradores globais também podem redefinir as senhas de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="26d8e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="26d8e-118">Certifique-se de entender os requisitos de licenciamento:</span><span class="sxs-lookup"><span data-stu-id="26d8e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="26d8e-119">Você deve ter pelo menos uma licença atribuída em sua organização:</span><span class="sxs-lookup"><span data-stu-id="26d8e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="26d8e-120">**Usuários somente na** nuvem - Qualquer SKU paga do Office 365 (O365) ou Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="26d8e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="26d8e-121">Usuários na nuvem **e/ou** locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="26d8e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="26d8e-122">Para saber mais sobre os requisitos de licenciamento, confira Requisitos de licenciamento para redefinição de senha de [autoatendado do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="26d8e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="26d8e-123">Para redefinir a senha de um usuário, encontre o usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="26d8e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="26d8e-124">Em seguida, na folha visão geral desse usuário, clique no botão "redefinir senha".</span><span class="sxs-lookup"><span data-stu-id="26d8e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="26d8e-125">**O botão de redefinição de senha está acinzentado**</span><span class="sxs-lookup"><span data-stu-id="26d8e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="26d8e-126">Você não está autorizado a **redefinir** as senhas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="26d8e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="26d8e-127">*Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.*</span><span class="sxs-lookup"><span data-stu-id="26d8e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="26d8e-128">Os administradores globais também podem redefinir as senhas de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="26d8e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="26d8e-129">**Não vejo a folha de redefinição de senha**</span><span class="sxs-lookup"><span data-stu-id="26d8e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="26d8e-130">Você não está autorizado a redefinir senhas.</span><span class="sxs-lookup"><span data-stu-id="26d8e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="26d8e-131">*Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.*</span><span class="sxs-lookup"><span data-stu-id="26d8e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="26d8e-132">Os administradores globais também podem redefinir as senhas de outros administradores privilegiados.</span><span class="sxs-lookup"><span data-stu-id="26d8e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="26d8e-133">**Não vejo a folha de integração local na redefinição de senha**</span><span class="sxs-lookup"><span data-stu-id="26d8e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="26d8e-134">A folha de integração local só aparece em ambientes híbridos, o que significa que você está usando o write-back de senha para manipular as senhas do usuário local.</span><span class="sxs-lookup"><span data-stu-id="26d8e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="26d8e-135">Você não verá essa folha se:</span><span class="sxs-lookup"><span data-stu-id="26d8e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="26d8e-136">Você não está usando write-back de senha</span><span class="sxs-lookup"><span data-stu-id="26d8e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="26d8e-137">Há um problema com a instalação/conectividade do write-back de senha</span><span class="sxs-lookup"><span data-stu-id="26d8e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="26d8e-138">Há um problema com sua instalação/conectividade do Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="26d8e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="26d8e-139">Para obter mais etapas de solução de problemas com o write-back de senha, consulte [Solucionar problemas de write-re de senha](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="26d8e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="26d8e-140">**Não sei como redefinir a senha de um usuário**</span><span class="sxs-lookup"><span data-stu-id="26d8e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="26d8e-141">Entre no portal do Azure como um administrador apropriado.</span><span class="sxs-lookup"><span data-stu-id="26d8e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="26d8e-142">Vá até a **folha Usuários e grupos,** selecione **Todos os Usuários.**</span><span class="sxs-lookup"><span data-stu-id="26d8e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="26d8e-143">Selecione um usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="26d8e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="26d8e-144">Para o usuário selecionado, selecione **Visão Geral** e, na barra de comandos, selecione **Redefinir senha.**</span><span class="sxs-lookup"><span data-stu-id="26d8e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="26d8e-145">Selecione o **botão Redefinir** senha e siga as instruções na tela.</span><span class="sxs-lookup"><span data-stu-id="26d8e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="26d8e-146">Somente redefinições realizadas por meio do **portal do Azure suportam** write-back de senha.</span><span class="sxs-lookup"><span data-stu-id="26d8e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="26d8e-147">**Redefini a senha de um usuário local do portal de administração do Office 365 ou do aplicativo móvel do Office 365, mas o usuário ainda não consegue entrar**</span><span class="sxs-lookup"><span data-stu-id="26d8e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="26d8e-148">O Write-back de senha não é suportado neste portal.</span><span class="sxs-lookup"><span data-stu-id="26d8e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="26d8e-149">Redefinir a senha do usuário novamente no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="26d8e-149">Reset the user's password again in the Azure portal.</span></span>

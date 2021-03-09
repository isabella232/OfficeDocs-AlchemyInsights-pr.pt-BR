---
title: Problema ao redefinir senha
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: fe3a13acb0ba5c8872d7c0bb8c3961d83f7d3526
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568434"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="2b5bd-102">Problemas para redefinir senha</span><span class="sxs-lookup"><span data-stu-id="2b5bd-102">Problems resetting password</span></span>

<span data-ttu-id="2b5bd-103">A seguir estão alguns dos problemas que você pode enfrentar ao redefinir a senha e as soluções possíveis:</span><span class="sxs-lookup"><span data-stu-id="2b5bd-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="2b5bd-104">**Estou tendo um problema com a redefinição de senha não abordada nas outras categorias**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

<span data-ttu-id="2b5bd-105">-Certifique-se de que você está autorizado a redefinir senhas.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-105">-Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="2b5bd-106">Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="2b5bd-107">Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="2b5bd-108">Certifique-se de entender os requisitos de licenciamento:</span><span class="sxs-lookup"><span data-stu-id="2b5bd-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="2b5bd-109">Você deve ter pelo menos uma licença atribuída em sua organização</span><span class="sxs-lookup"><span data-stu-id="2b5bd-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="2b5bd-110">Usuários somente na nuvem - Qualquer SKU pago do Office 365 (O365) ou do Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="2b5bd-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="2b5bd-111">Usuários na nuvem e/ou locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="2b5bd-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="2b5bd-112">Para ler mais sobre os requisitos de licenciamento, consulte o artigo Requisitos de licenciamento para a redefinição de senha de [autoatendados do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="2b5bd-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="2b5bd-113">**Estou com problemas para testar a política de redefinição de senha que defina**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="2b5bd-114">Políticas aplicadas recentemente podem levar vários minutos para replicar em todos os data centers e pontos de extremidade.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="2b5bd-115">A distância física do data center também afetará a rapidez com que as alterações são aplicadas.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="2b5bd-116">Teste com um usuário final, não um administrador e piloto com um pequeno conjunto de usuários.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="2b5bd-117">As políticas configuradas no portal do Azure APLICAM-se SOMENTE aos usuários finais, não aos administradores.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="2b5bd-118">A Microsoft impõe uma política de redefinição de senha de dois portais padrão forte para qualquer função de administrador do Azure (Exemplo: Administrador Global, Administrador de Ajuda, Administrador de Senha etc.)</span><span class="sxs-lookup"><span data-stu-id="2b5bd-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="2b5bd-119">Saiba mais sobre [políticas para administradores.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="2b5bd-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="2b5bd-120">**Quero implantar a redefinição de senha, mas não quero que meus usuários registrem informações adicionais de segurança**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="2b5bd-121">Preencher previamente dados para seus usuários para que eles não tenham que fazer isso!</span><span class="sxs-lookup"><span data-stu-id="2b5bd-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="2b5bd-122">- Como administrador, você pode definir propriedades de telefone e email para seus usuários antes de fazer a redefinição de senha para sua organização.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="2b5bd-123">Você pode fazer isso usando uma API, PowerShell ou Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="2b5bd-124">Mais informações aqui:</span><span class="sxs-lookup"><span data-stu-id="2b5bd-124">More information here:</span></span>
- [<span data-ttu-id="2b5bd-125">Implantando redefinição de senha sem exigir que os usuários se registrem</span><span class="sxs-lookup"><span data-stu-id="2b5bd-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="2b5bd-126">Quais dados são usados pela redefinição de senha</span><span class="sxs-lookup"><span data-stu-id="2b5bd-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="2b5bd-127">**O botão de redefinição de senha está acinzentado**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="2b5bd-128">Você não está autorizado a redefinir as senhas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="2b5bd-129">Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="2b5bd-130">Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2b5bd-131">**Não vejo a folha de redefinição de senha**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="2b5bd-132">Você não está autorizado a redefinir senhas.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="2b5bd-133">Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="2b5bd-134">Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2b5bd-135">**Não vejo a folha de integração local na redefinição de senha**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="2b5bd-136">A folha de integração local só aparece em ambientes híbridos , o que significa que você está usando o writeback de senha para manipular as senhas do usuário local.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="2b5bd-137">Você não verá essa folha se:</span><span class="sxs-lookup"><span data-stu-id="2b5bd-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="2b5bd-138">Você não está usando writeback de senha</span><span class="sxs-lookup"><span data-stu-id="2b5bd-138">You are not using password writeback</span></span>
    - <span data-ttu-id="2b5bd-139">Há um problema com a instalação/conectividade do writeback de senha</span><span class="sxs-lookup"><span data-stu-id="2b5bd-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="2b5bd-140">Há um problema com sua instalação/conectividade do Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="2b5bd-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="2b5bd-141">Para obter mais etapas de solução de problemas para problemas com o writeback de senha, consulte a seção [Solucionar problemas de writeback de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="2b5bd-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="2b5bd-142">**Não sei como redefinir a senha de um usuário**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="2b5bd-143">Entre no portal do Azure como um administrador apropriado.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="2b5bd-144">Vá para a folha Usuários e grupos, selecione **Todos os Usuários**.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="2b5bd-145">Selecione um usuário na lista.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-145">Select a user from the list.</span></span>
1. <span data-ttu-id="2b5bd-146">Para o usuário selecionado, selecione **Visão Geral** e, em seguida, na barra de comandos, clique em **Redefinir senha**.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="2b5bd-147">Siga as instruções na tela.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="2b5bd-148">Somente as redefinições realizadas por meio do portal do Azure suportam o writeback de senha.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="2b5bd-149">**Redefini a senha de um usuário local do portal de administração do Office 365 ou do aplicativo móvel do Office 365, mas o usuário ainda não consegue entrar**</span><span class="sxs-lookup"><span data-stu-id="2b5bd-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="2b5bd-150">O Writeback de senha não é suportado neste portal.</span><span class="sxs-lookup"><span data-stu-id="2b5bd-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="2b5bd-151">Redefinir a senha do usuário novamente no portal do Azure - portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="2b5bd-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>


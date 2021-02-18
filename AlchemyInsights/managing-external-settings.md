---
title: Gerenciando configurações externas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282800"
---
# <a name="managing-external-settings"></a><span data-ttu-id="603e7-102">Gerenciando configurações externas</span><span class="sxs-lookup"><span data-stu-id="603e7-102">Managing External Settings</span></span>

<span data-ttu-id="603e7-103">**Comunicado**</span><span class="sxs-lookup"><span data-stu-id="603e7-103">**Announcement**</span></span>

- <span data-ttu-id="603e7-104">[Suspensão do suporte de login do WebView do Google a partir de 4 de janeiro de 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="603e7-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="603e7-105">Teste se seus aplicativos são afetados seguindo as orientações do Google sobre o teste de compatibilidade</span><span class="sxs-lookup"><span data-stu-id="603e7-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="603e7-106">Certifique-se de usar o webview do sistema ou o navegador do sistema ao conectar seus usuários com contas pessoais do Google</span><span class="sxs-lookup"><span data-stu-id="603e7-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="603e7-107">**Gerenciar configurações de convite**</span><span class="sxs-lookup"><span data-stu-id="603e7-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="603e7-108">Confirme se você [definiu as configurações de colaboração externa](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) para permitir que as pessoas apropriadas enviem convites.</span><span class="sxs-lookup"><span data-stu-id="603e7-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="603e7-109">**Gerenciar permissões de acesso de usuário convidado**</span><span class="sxs-lookup"><span data-stu-id="603e7-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="603e7-110">Os administradores globais podem gerenciar permissões de acesso de convidado no diretório por meio do portal do Azure, configurando as permissões de acesso de convidado na página Configurações de colaboração externa.</span><span class="sxs-lookup"><span data-stu-id="603e7-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="603e7-111">[Saiba mais sobre essa configuração](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="603e7-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="603e7-112">Se quiser que seus convidados acessem aplicativos como Teams ou Microsoft Office SharePoint Online, confirme se você configurou esses aplicativos para permitir o acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="603e7-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="603e7-113">Saiba mais sobre as configurações [das equipes](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) e [do Microsoft Office SharePoint Online](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="603e7-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="603e7-114">**Configurando convites:**</span><span class="sxs-lookup"><span data-stu-id="603e7-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="603e7-115">Habilite a colaboração externa B2B e gerencie quem pode convidar pessoas</span><span class="sxs-lookup"><span data-stu-id="603e7-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="603e7-116">Permitir ou bloquear convites para usuários de organizações específicas</span><span class="sxs-lookup"><span data-stu-id="603e7-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="603e7-117">**Configurando provedores de identidade permitidos:**</span><span class="sxs-lookup"><span data-stu-id="603e7-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="603e7-118">Federação Google</span><span class="sxs-lookup"><span data-stu-id="603e7-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="603e7-119">Federação Direta</span><span class="sxs-lookup"><span data-stu-id="603e7-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="603e7-120">Autenticação de senha única de email</span><span class="sxs-lookup"><span data-stu-id="603e7-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)

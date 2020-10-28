---
title: Acesso à assinatura
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773767"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="ee04f-102">Não é possível entrar no Azure devido a problemas de navegador (o navegador trava, continua girando, não carrega, etc.)</span><span class="sxs-lookup"><span data-stu-id="ee04f-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="ee04f-103">Você pode ser afetado por uma interrupção.</span><span class="sxs-lookup"><span data-stu-id="ee04f-103">You might be impacted by an outage.</span></span> <span data-ttu-id="ee04f-104">Verifique se há uma interrupção em andamento: [status de integridade do Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="ee04f-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="ee04f-105">Faça logoff de todas as sessões ativas do Azure.</span><span class="sxs-lookup"><span data-stu-id="ee04f-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="ee04f-106">Inicie um modo in-private ou incógnito do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="ee04f-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="ee04f-107">Você também pode tentar atualizar o navegador, usar outro navegador, Excluir cookies de cache se acima não funcionar.</span><span class="sxs-lookup"><span data-stu-id="ee04f-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="ee04f-108">Saiba mais: [solucionar problemas de entrada](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="ee04f-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="ee04f-109">**Não é possível acessar assinaturas**</span><span class="sxs-lookup"><span data-stu-id="ee04f-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="ee04f-110">No [portal do Azure](https://portal.azure.com/), certifique-se de que o diretório do Azure correto está selecionado na conta no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="ee04f-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="ee04f-111">No [centro de contas do Azure](https://account.windowsazure.com/Subscriptions), certifique-se de que a conta usada seja o administrador da conta.</span><span class="sxs-lookup"><span data-stu-id="ee04f-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="ee04f-112">Saiba mais: [solucionar problemas de nenhuma assinatura encontrada](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ee04f-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="ee04f-113">**Não é possível acessar o histórico de cobrança**</span><span class="sxs-lookup"><span data-stu-id="ee04f-113">**Unable to access billing history**</span></span>

<span data-ttu-id="ee04f-114">O administrador da conta precisa certificar-se de que o usuário que estiver acessando as informações de cobrança seja adicionado ao Azure Active Directory como um usuário convidado: [Adicionar ou excluir um novo usuário](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ee04f-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ee04f-115">Em seguida, o usuário deve receber uma função de administrador global: [atribuir função aos usuários](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ee04f-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ee04f-116">Postar isso, o usuário pode receber acesso de cobrança usando políticas RBAC: [conceder acesso à cobrança](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ee04f-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ee04f-117">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="ee04f-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="ee04f-118">Não consigo entrar para gerenciar minha assinatura do Azure</span><span class="sxs-lookup"><span data-stu-id="ee04f-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)
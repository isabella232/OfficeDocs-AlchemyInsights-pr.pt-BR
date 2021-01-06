---
title: Como adicionar e gerenciar os administradores-etapas recomendadas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755823"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="6b29e-102">Como adicionar e gerenciar os administradores-etapas recomendadas</span><span class="sxs-lookup"><span data-stu-id="6b29e-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="6b29e-103">Com base na descrição do problema, encontramos uma solução para você.</span><span class="sxs-lookup"><span data-stu-id="6b29e-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="6b29e-104">A maioria dos clientes foi capaz de resolver seu problema por conta própria após seguir nossa documentação.</span><span class="sxs-lookup"><span data-stu-id="6b29e-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="6b29e-105">**Editar o administrador de assinaturas ou coadministrador**</span><span class="sxs-lookup"><span data-stu-id="6b29e-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="6b29e-106">O administrador da conta pode editar as duas funções, enquanto o administrador de assinaturas só pode alterar os coadministradores no [portal do Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="6b29e-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="6b29e-107">Adicionar ou alterar administradores de assinatura do Azure</span><span class="sxs-lookup"><span data-stu-id="6b29e-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="6b29e-108">**Atualizar o administrador de assinaturas ou Co-Administrator para assinaturas internas (TRANSMITIdas)**</span><span class="sxs-lookup"><span data-stu-id="6b29e-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="6b29e-109">O administrador de serviço ou o coadministrador pode atender a essa ação usando as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="6b29e-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="6b29e-110">Faça logon no [portal do Azure](https://ms.portal.azure.com/#home) e clique em **Gerenciamento de custos + cobrança** na folha esquerda.</span><span class="sxs-lookup"><span data-stu-id="6b29e-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="6b29e-111">Clique no item de linha com sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="6b29e-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="6b29e-112">Isso abre a visão geral da sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="6b29e-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="6b29e-113">Na folha **assinatura** , clique em **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="6b29e-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="6b29e-114">Clique no botão **administrador de serviços** .</span><span class="sxs-lookup"><span data-stu-id="6b29e-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="6b29e-115">Insira o email do usuário que você deseja definir como administrador de serviço e clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="6b29e-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="6b29e-116">**Adicionar/Alterar/remover coadministrador**</span><span class="sxs-lookup"><span data-stu-id="6b29e-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="6b29e-117">Faça logon no [portal do Azure](https://ms.portal.azure.com/#home) como um administrador de serviço.</span><span class="sxs-lookup"><span data-stu-id="6b29e-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="6b29e-118">Abra [assinaturas](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) e selecione uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="6b29e-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="6b29e-119">(Coadministradores só podem ser atribuídos no escopo de assinatura.)</span><span class="sxs-lookup"><span data-stu-id="6b29e-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="6b29e-120">Navegue até **controle de acesso (iam)**  >  **os administradores clássicos**  >  **Add**  >  **Add coadministrador** para abrir o painel **Adicionar** coadministrador (se a opção Adicionar coadministrador estiver desabilitada, ela indica que você não tem permissões).</span><span class="sxs-lookup"><span data-stu-id="6b29e-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="6b29e-121">Selecione o usuário que você deseja adicionar e clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="6b29e-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="6b29e-122">**Saiba Mais:**</span><span class="sxs-lookup"><span data-stu-id="6b29e-122">**Learn more:**</span></span>
- [<span data-ttu-id="6b29e-123">Adicionar um coadministrador</span><span class="sxs-lookup"><span data-stu-id="6b29e-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="6b29e-124">Remover um coadministrador</span><span class="sxs-lookup"><span data-stu-id="6b29e-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="6b29e-125">Alterar o administrador de serviço</span><span class="sxs-lookup"><span data-stu-id="6b29e-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="6b29e-126">Exibir o administrador da conta</span><span class="sxs-lookup"><span data-stu-id="6b29e-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="6b29e-127">Gerenciar o acesso usando o RBAC e o portal do Azure</span><span class="sxs-lookup"><span data-stu-id="6b29e-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="6b29e-128">**Adicionar/excluir usuários usando o Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="6b29e-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="6b29e-129">Você pode adicionar novos usuários ou excluir usuários existentes da organização do Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="6b29e-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="6b29e-130">Para adicionar um novo usuário, faça logon no [portal do Azure](https://ms.portal.azure.com/#home) como administrador de usuário da organização.</span><span class="sxs-lookup"><span data-stu-id="6b29e-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="6b29e-131">Selecione **Azure Active Directory**, selecione **usuários** e, em seguida, clique em **novo usuário**.</span><span class="sxs-lookup"><span data-stu-id="6b29e-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="6b29e-132">Na página do **usuário** , preencha as informações necessárias.</span><span class="sxs-lookup"><span data-stu-id="6b29e-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="6b29e-133">Clique em **Criar**.</span><span class="sxs-lookup"><span data-stu-id="6b29e-133">Click **Create**.</span></span> <span data-ttu-id="6b29e-134">O usuário é criado e adicionado ao seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6b29e-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="6b29e-135">**Saiba mais**:</span><span class="sxs-lookup"><span data-stu-id="6b29e-135">**Learn more**:</span></span>

- [<span data-ttu-id="6b29e-136">Adicionar um novo usuário</span><span class="sxs-lookup"><span data-stu-id="6b29e-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="6b29e-137">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="6b29e-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="6b29e-138">Adicionar ou atualizar as informações de perfil de um usuário usando o Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6b29e-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="6b29e-139">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="6b29e-139">**Recommended documents**</span></span>

- [<span data-ttu-id="6b29e-140">O que é controle de acesso baseado em função (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="6b29e-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="6b29e-141">Entender as diferentes funções no Azure</span><span class="sxs-lookup"><span data-stu-id="6b29e-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="6b29e-142">Permissões da função de administrador no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6b29e-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="6b29e-143">Tutorial: conceder acesso a um usuário usando o RBAC e o portal do Azure</span><span class="sxs-lookup"><span data-stu-id="6b29e-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="6b29e-144">Solucionar problemas de RBAC no Azure</span><span class="sxs-lookup"><span data-stu-id="6b29e-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="6b29e-145">Organizar seus recursos com grupos de gerenciamento do Azure</span><span class="sxs-lookup"><span data-stu-id="6b29e-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="6b29e-146">Como solicitar a cópia da fatura do Azure via email</span><span class="sxs-lookup"><span data-stu-id="6b29e-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="6b29e-147">Como adicionar, atualizar ou remover um cartão de crédito ou débito do Azure</span><span class="sxs-lookup"><span data-stu-id="6b29e-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="6b29e-148">Gerenciar a assinatura (reativar/cancelar/alternar)</span><span class="sxs-lookup"><span data-stu-id="6b29e-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




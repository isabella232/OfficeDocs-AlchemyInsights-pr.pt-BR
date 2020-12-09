---
title: Habilitar gerenciamento de custos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599045"
---
# <a name="enable-cost-management"></a><span data-ttu-id="14abf-102">Habilitar gerenciamento de custos</span><span class="sxs-lookup"><span data-stu-id="14abf-102">Enable cost management</span></span>

<span data-ttu-id="14abf-103">**O que os custos estão desabilitados para a sua organização?**</span><span class="sxs-lookup"><span data-stu-id="14abf-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="14abf-104">As organizações que usam as contas do Enterprise Agreement (EA) ou da Microsoft Customer Agreement (MCA) podem desabilitar o acesso a informações de custo e informações de preços.</span><span class="sxs-lookup"><span data-stu-id="14abf-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="14abf-105">Após fazer logon no portal do Azure, eles podem usar as APIs de cobrança para obter faturas programaticamente (depois de optar) e detalhes de uso.</span><span class="sxs-lookup"><span data-stu-id="14abf-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="14abf-106">**Como permitir que usuários adicionais acessem faturas**</span><span class="sxs-lookup"><span data-stu-id="14abf-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="14abf-107">Vá para a **folha de assinaturas** no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="14abf-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="14abf-108">Selecione **faturas** e, em seguida, **acesso a faturas**.</span><span class="sxs-lookup"><span data-stu-id="14abf-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="14abf-109">Ative o acesso, seguido salvando as alterações, para permitir que os usuários em funções com escopo de assinatura baixem faturas.</span><span class="sxs-lookup"><span data-stu-id="14abf-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="14abf-110">O administrador da conta também pode configurar o para ter faturas enviadas por email.</span><span class="sxs-lookup"><span data-stu-id="14abf-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="14abf-111">Para saber mais, confira [obter sua fatura por email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="14abf-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="14abf-112">**Como adicionar usuários à função leitor de cobrança**</span><span class="sxs-lookup"><span data-stu-id="14abf-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="14abf-113">Vá para a **folha de assinaturas** no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="14abf-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="14abf-114">Selecione **controle de acesso (iam)** e clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="14abf-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="14abf-115">Escolha **leitor de cobrança** na página **selecionar uma função** .</span><span class="sxs-lookup"><span data-stu-id="14abf-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="14abf-116">Digite o email do usuário que você deseja convidar e, em seguida, clique em **OK** para enviar o convite.</span><span class="sxs-lookup"><span data-stu-id="14abf-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="14abf-117">Siga as instruções fornecidas no email de convite para fazer logon como um leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="14abf-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="14abf-118">Para obter mais informações, consulte [conceder acesso à cobrança](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="14abf-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="14abf-119">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="14abf-119">**Recommended documents**</span></span>

- [<span data-ttu-id="14abf-120">Habilitar modos de exibição DA e ao via portal de EA</span><span class="sxs-lookup"><span data-stu-id="14abf-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="14abf-121">Custos incluídos no gerenciamento de custos</span><span class="sxs-lookup"><span data-stu-id="14abf-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="14abf-122">Ofertas compatíveis com o Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="14abf-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="14abf-123">Analisar custos na análise de custo</span><span class="sxs-lookup"><span data-stu-id="14abf-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="14abf-124">Fornecer acesso a informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="14abf-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="14abf-125">Verificar acesso a um contrato de cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="14abf-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)







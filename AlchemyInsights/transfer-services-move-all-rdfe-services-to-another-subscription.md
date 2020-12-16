---
title: Serviços de transferência-mover todos os serviços RDFE para outra assinatura
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681446"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="aec35-102">Serviços de transferência-mover todos os serviços RDFE para outra assinatura</span><span class="sxs-lookup"><span data-stu-id="aec35-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="aec35-103">**Mover recursos**</span><span class="sxs-lookup"><span data-stu-id="aec35-103">**Move resources**</span></span>

<span data-ttu-id="aec35-104">Os recursos do Azure podem ser movidos para outra assinatura do Azure ou grupo de recursos na mesma assinatura usando o portal do Azure, o Azure PowerShell, o Azure CLI ou a API REST para mover recursos.</span><span class="sxs-lookup"><span data-stu-id="aec35-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="aec35-105">Antes de poder mover recursos, consulte:</span><span class="sxs-lookup"><span data-stu-id="aec35-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="aec35-106">Lista de verificação antes de mover os recursos</span><span class="sxs-lookup"><span data-stu-id="aec35-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="aec35-107">Serviços que podem ser movidos</span><span class="sxs-lookup"><span data-stu-id="aec35-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="aec35-108">Como validar a movimentação</span><span class="sxs-lookup"><span data-stu-id="aec35-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="aec35-109">Diretrizes de movimentação para serviços</span><span class="sxs-lookup"><span data-stu-id="aec35-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="aec35-110">Para mover recursos existentes para outro grupo de recursos ou assinatura, você pode usar:</span><span class="sxs-lookup"><span data-stu-id="aec35-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="aec35-111">Portal do Azure</span><span class="sxs-lookup"><span data-stu-id="aec35-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="aec35-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="aec35-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="aec35-113">CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="aec35-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="aec35-114">API REST</span><span class="sxs-lookup"><span data-stu-id="aec35-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="aec35-115">Tutorial: [mover recursos do Azure para outro grupo de recursos ou assinatura](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="aec35-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="aec35-116">**Solucionar erros com o Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="aec35-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="aec35-117">Consulte os artigos abaixo para saber mais sobre alguns erros comuns de implantação do Azure e receber informações para resolvê-los.</span><span class="sxs-lookup"><span data-stu-id="aec35-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="aec35-118">Se você não conseguir encontrar o código de erro para o erro de implantação, confira [Localizar código de erro](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="aec35-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="aec35-119">Solucionar erros de implantação</span><span class="sxs-lookup"><span data-stu-id="aec35-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="aec35-120">Solucionar problemas de movimentação de recursos do Azure para o novo grupo de recursos ou assinatura</span><span class="sxs-lookup"><span data-stu-id="aec35-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="aec35-121">Observe que, se você quiser atualizar sua assinatura do Azure, como mudar de gratuita para pagar conforme o ponto, precisará converter sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="aec35-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="aec35-122">Para atualizar uma avaliação gratuita, confira [atualizar sua assinatura de avaliação gratuita ou Microsoft imagine Azure para o pagamento conforme a ser acessado](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="aec35-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="aec35-123">Para alterar uma conta de pagamento conforme você, confira [alterar sua assinatura de pagamento a ser direcionado do Azure para uma oferta diferente](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="aec35-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="aec35-124">**Para adicionar ou associar uma assinatura do Azure ao seu locatário do Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="aec35-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="aec35-125">Entre e selecione a assinatura que você deseja usar na [página assinaturas no portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="aec35-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="aec35-126">Selecione **Alterar diretório**.</span><span class="sxs-lookup"><span data-stu-id="aec35-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="aec35-127">Revise todos os avisos exibidos e selecione **alterar**.</span><span class="sxs-lookup"><span data-stu-id="aec35-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="aec35-128">O diretório é alterado para a assinatura e você receberá uma mensagem de êxito.</span><span class="sxs-lookup"><span data-stu-id="aec35-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="aec35-129">Use o seletor de *diretório* para ir para o novo diretório.</span><span class="sxs-lookup"><span data-stu-id="aec35-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="aec35-130">Pode levar até 10 minutos para que tudo seja exibido corretamente.</span><span class="sxs-lookup"><span data-stu-id="aec35-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="aec35-131">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="aec35-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="aec35-132">Transferindo a propriedade de uma assinatura do Azure</span><span class="sxs-lookup"><span data-stu-id="aec35-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="aec35-133">Mover recursos para o novo grupo de recursos ou assinatura</span><span class="sxs-lookup"><span data-stu-id="aec35-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="aec35-134">Gerenciar recursos usando o portal do Azure</span><span class="sxs-lookup"><span data-stu-id="aec35-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)

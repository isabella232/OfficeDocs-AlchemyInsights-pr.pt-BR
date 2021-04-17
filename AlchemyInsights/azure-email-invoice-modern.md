---
title: Faturamento por email moderno do Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820814"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="ba0d6-102">Faturamento por email no Azure</span><span class="sxs-lookup"><span data-stu-id="ba0d6-102">Email invoicing in Azure</span></span>

<span data-ttu-id="ba0d6-103">Você deve ter uma função de proprietário ou contribuidor no perfil de cobrança ou em sua conta de cobrança para atualizar sua preferência de fatura por email.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="ba0d6-104">Depois de ter ativado, todos os usuários com funções de proprietário, contribuidor, leitores e gerenciador de faturas em um perfil de cobrança receberão sua fatura por email.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="ba0d6-105">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ba0d6-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="ba0d6-106">Pesquise por **Gerenciamento de Custos + Cobrança**.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="ba0d6-107">Selecione **Faturas** no lado esquerdo e, em seguida, selecione **Fatura por email** no topo da página.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="ba0d6-108">Se você tiver vários perfis de cobrança, selecione um perfil de cobrança e selecione **Aceitar**.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="ba0d6-109">Selecione **Atualizar**.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-109">Select **Update**.</span></span>
6. <span data-ttu-id="ba0d6-110">Se você tiver vários perfis de cobrança, selecione um perfil de cobrança e selecione **Aceitar**.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="ba0d6-111">Você concede a outros acesso para exibir, baixar e pagar faturas atribuindo-lhes a função de gerenciador de faturas para um perfil de cobrança MCA ou MPA.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="ba0d6-112">Se você optou por obter sua fatura por email, os usuários também obterão as faturas por email.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="ba0d6-113">Entre no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ba0d6-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="ba0d6-114">Pesquise por **Gerenciamento de Custos + Cobrança**.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="ba0d6-115">Selecione **Perfis de cobrança** do lado esquerdo.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="ba0d6-116">Na lista de perfis de cobrança, selecione um perfil de cobrança ao qual deseja atribuir uma função de gerente de fatura.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="ba0d6-117">Selecione **Controle de acesso (IAM)** no lado esquerdo e selecione **Adicionar** no topo da página.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="ba0d6-118">Na lista suspensa de Função, selecione **Gerenciador de faturas**.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="ba0d6-119">Insira o endereço de email do usuário para conceder acesso.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="ba0d6-120">Selecione **Salvar** para atribuir a função.</span><span class="sxs-lookup"><span data-stu-id="ba0d6-120">Select **Save** to assign the role.</span></span>

---
title: Transferir propriedade de cobrança do Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840566"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="13067-102">Transferir propriedade de cobrança do Azure</span><span class="sxs-lookup"><span data-stu-id="13067-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="13067-103">Entre no [portal do Azure](https://portal.azure.com/) como administrador da conta de cobrança que possui a assinatura que deseja transferir.</span><span class="sxs-lookup"><span data-stu-id="13067-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="13067-104">Se não tiver certeza se você é o administrador ou se precisa determinar quem é, confira [Determinar o administrador de cobrança da conta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="13067-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="13067-105">Pesquise em **Gerenciamento de Custos + Cobrança**.</span><span class="sxs-lookup"><span data-stu-id="13067-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="13067-106">Selecione **Assinaturas** no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="13067-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="13067-107">Dependendo do acesso, você pode precisar selecionar um escopo de cobrança e, em seguida, **Assinaturas** ou **Assinaturas do Azure**.</span><span class="sxs-lookup"><span data-stu-id="13067-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="13067-108">Selecione **Transferir propriedade de cobrança** para a assinatura que deseja transferir</span><span class="sxs-lookup"><span data-stu-id="13067-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="13067-109">Insira o endereço de e-mail de um usuário que é administrador de cobrança da conta e será o novo proprietário da assinatura e selecione **enviar solicitação de transferência**</span><span class="sxs-lookup"><span data-stu-id="13067-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="13067-110">O usuário recebe um email com instruções para revisar sua solicitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="13067-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="13067-111">Para aprovar a solicitação de transferência, o usuário seleciona o link no email e segue as instruções.</span><span class="sxs-lookup"><span data-stu-id="13067-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="13067-112">**Observação** : Se você transferir a propriedade de cobrança de sua assinatura para uma conta de usuário em outro locatário do Azure Active Directory, todas as atribuições de [controle de acesso baseado em função (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para gerenciar recursos na assinatura serão permanentemente removido.</span><span class="sxs-lookup"><span data-stu-id="13067-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="13067-113">Somente o novo proprietário terá acesso ao gerenciamento de recursos na assinatura.</span><span class="sxs-lookup"><span data-stu-id="13067-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="13067-114">Para saber mais, confira [Transferindo a assinatura para um usuário em outro locatário do Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="13067-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="13067-115">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="13067-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="13067-116">Transferir a propriedade de cobrança de uma assinatura do Azure para outra conta</span><span class="sxs-lookup"><span data-stu-id="13067-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="13067-117">Sobre a transferência de propriedade de cobrança para uma assinatura do Azure</span><span class="sxs-lookup"><span data-stu-id="13067-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="13067-118">Transferindo o Microsoft Visual Studio, Microsoft Partner Network (MPN) e assinaturas de desenvolvimento/teste Pré-pagos</span><span class="sxs-lookup"><span data-stu-id="13067-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="13067-119">Perguntas frequentes sobre Transferência de Propriedade</span><span class="sxs-lookup"><span data-stu-id="13067-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="13067-120">Solucionar problemas de Transferência de Propriedade</span><span class="sxs-lookup"><span data-stu-id="13067-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

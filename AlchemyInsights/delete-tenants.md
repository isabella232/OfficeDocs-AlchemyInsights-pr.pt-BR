---
title: Excluir locatário
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477641"
---
# <a name="delete-tenant"></a><span data-ttu-id="cd863-102">Excluir locatário</span><span class="sxs-lookup"><span data-stu-id="cd863-102">Delete tenant</span></span>

<span data-ttu-id="cd863-103">Para excluir um Azure AD, verifique se:</span><span class="sxs-lookup"><span data-stu-id="cd863-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="cd863-104">Você é um administrador global no diretório.</span><span class="sxs-lookup"><span data-stu-id="cd863-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="cd863-105">Você não está conectado com uma conta que tenha o diretório padrão como contoso.onmicrosoft.com na conta de entrada, como admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="cd863-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="cd863-106">Remova quaisquer aplicativos ativos no diretório antes da exclusão.</span><span class="sxs-lookup"><span data-stu-id="cd863-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="cd863-107">Para remover aplicativos ativos, navegue até registros de aplicativos e remova os aplicativos existentes.</span><span class="sxs-lookup"><span data-stu-id="cd863-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="cd863-108">Não há assinaturas ativas para os serviços online da Microsoft, como o Microsoft Azure, o Office 365 ou o Azure AD Premium associado ao diretório.</span><span class="sxs-lookup"><span data-stu-id="cd863-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="cd863-109">Transferir suas assinaturas ou agilizar o cancelamento de assinaturas ativas por meio de suporte e cobrança do Azure.</span><span class="sxs-lookup"><span data-stu-id="cd863-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="cd863-110">Saiba mais sobre como cancelar assinaturas do Office 365 e do Azure.</span><span class="sxs-lookup"><span data-stu-id="cd863-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="cd863-111">Para obter orientação sobre como associar ou adicionar uma assinatura existente a um locatário, confira [associar ou adicionar uma assinatura do Azure ao seu locatário do Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="cd863-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="cd863-112">Não há licença ativa.</span><span class="sxs-lookup"><span data-stu-id="cd863-112">There are no Active license.</span></span> <span data-ttu-id="cd863-113">Para remover licenças, consulte [How to remove Subscription for remove License](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="cd863-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="cd863-114">Não há outros usuários ativos no diretório, além de ser o administrador global ao tentar excluir o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cd863-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="cd863-115">Remova outros usuários ativos, e quaisquer dependências em um nome de domínio personalizado no locatário também precisarão ser removidas, como os usuários criados com o admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="cd863-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="cd863-116">Para obter mais detalhes sobre como:</span><span class="sxs-lookup"><span data-stu-id="cd863-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="cd863-117">Delete "Azure Active Directory" ou "Subscription", consulte [delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="cd863-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="cd863-118">Removendo aplicativos no diretório, consulte [removendo aplicativos](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="cd863-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 

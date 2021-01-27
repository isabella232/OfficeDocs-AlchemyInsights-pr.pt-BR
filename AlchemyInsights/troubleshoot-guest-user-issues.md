---
title: Solucionar problemas de usuários convidados
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897681"
---
# <a name="troubleshoot-guest-user-issues"></a><span data-ttu-id="ede41-102">Solucionar problemas de usuários convidados</span><span class="sxs-lookup"><span data-stu-id="ede41-102">Troubleshoot guest user issues</span></span>

1. <span data-ttu-id="ede41-103">Para obter orientações sobre como gerenciar o acesso de convidados a aplicativos, confira Gerenciar o acesso de convidados com revisões de acesso [do Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)</span><span class="sxs-lookup"><span data-stu-id="ede41-103">For guidance on managing guest access to applications, see [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).</span></span>
1. <span data-ttu-id="ede41-104">Adicione usuários convidados ao seu diretório no portal do [Azure:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)neste guia de início rápido, você adicionará um novo usuário convidado ao diretório do Azure AD por meio do portal do Azure, enviará um convite e verá a aparência do processo de resgate do convite do usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="ede41-104">[Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): In this quickstart, you'll add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
1. <span data-ttu-id="ede41-105">Adicione um usuário convidado com [o PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)neste guia de início rápido, você usará o comando New-AzureADMSInvitation para adicionar um usuário convidado ao seu locatário do Azure.</span><span class="sxs-lookup"><span data-stu-id="ede41-105">[Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): In this quickstart, you’ll use the New-AzureADMSInvitation command to add one guest user to your Azure tenant.</span></span>
1. <span data-ttu-id="ede41-106">Para saber como atribuir usuários e grupos a aplicativos empresariais no Azure Active Directory (Azure AD), de dentro do portal do Azure ou usando o PowerShell, confira Gerenciar a atribuição de usuário para um aplicativo no [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)</span><span class="sxs-lookup"><span data-stu-id="ede41-106">To learn how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span> 
1. <span data-ttu-id="ede41-107">A colaboração B2B do Azure Active Directory (Azure AD) funciona com a maioria dos aplicativos que se integram ao Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ede41-107">Azure Active Directory (Azure AD) B2B collaboration works with most apps that integrate with Azure AD.</span></span> <span data-ttu-id="ede41-108">Neste [artigo,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)vamos ver as instruções para configurar alguns aplicativos SaaS populares para uso com o Azure AD B2B.</span><span class="sxs-lookup"><span data-stu-id="ede41-108">In this [article](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), we walk through instructions for configuring some popular SaaS apps for use with Azure AD B2B.</span></span>
1. <span data-ttu-id="ede41-109">Como uma organização que usa os recursos de colaboração B2B do Azure Active Directory (Azure AD) para convidar usuários convidados de organizações parceiras para o Azure AD, agora você pode fornecer a esses usuários B2B acesso a aplicativos locais.</span><span class="sxs-lookup"><span data-stu-id="ede41-109">As an organization that uses Azure Active Directory (Azure AD) B2B collaboration capabilities to invite guest users from partner organizations to your Azure AD, you can now provide these B2B users access to on-premises apps.</span></span> <span data-ttu-id="ede41-110">Esses aplicativos locais podem usar a autenticação baseada em SAML ou a Autenticação Integrada do Windows (IWA) com kCD (delegação restrita de Kerberos).</span><span class="sxs-lookup"><span data-stu-id="ede41-110">These on-premises apps can use SAML-based authentication or Integrated Windows Authentication (IWA) with Kerberos constrained delegation (KCD).</span></span> <span data-ttu-id="ede41-111">Para saber mais, confira Conceder aos usuários [B2B no Azure AD acesso aos seus aplicativos locais.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)</span><span class="sxs-lookup"><span data-stu-id="ede41-111">For more information, see [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).</span></span>
1. <span data-ttu-id="ede41-112">Saiba como conceder acesso a contas de parceiros gerenciadas localmente para recursos de nuvem [usando a colaboração B2B do Azure AD.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)</span><span class="sxs-lookup"><span data-stu-id="ede41-112">Learn how to [grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).</span></span>
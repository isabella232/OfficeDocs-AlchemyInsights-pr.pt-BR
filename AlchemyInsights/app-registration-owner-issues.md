---
title: Problemas do Proprietário do Registro de Aplicativos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123032"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="9e98e-102">Problemas do Proprietário do Registro de Aplicativos</span><span class="sxs-lookup"><span data-stu-id="9e98e-102">App Registration Owner issues</span></span>

<span data-ttu-id="9e98e-103">A seguir estão os métodos disponíveis para adicionar entidades como proprietários para registros de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="9e98e-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="9e98e-104">Usando o módulo powershell do Azure AD -</span><span class="sxs-lookup"><span data-stu-id="9e98e-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="9e98e-105">Referência: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="9e98e-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="9e98e-106">Usando a CLI do Azure - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="9e98e-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="9e98e-107">Referência: [proprietário do aplicativo do az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="9e98e-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="9e98e-108">Usando o MS Graph -</span><span class="sxs-lookup"><span data-stu-id="9e98e-108">Using MS Graph -</span></span>

    <span data-ttu-id="9e98e-109">Referência: [Adicionar proprietário - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="9e98e-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="9e98e-110">Usando o Portal do Azure AD - Navegue até portal.azure.com [>](https://portal.azure.com/) Azure Active directory > App Registration > Selecione seu aplicativo > Proprietários > Adicionar Proprietários</span><span class="sxs-lookup"><span data-stu-id="9e98e-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="9e98e-111">**Não é possível exibir seu aplicativo na folha Registros de Aplicativos, mesmo que você seja o proprietário desse aplicativo?**</span><span class="sxs-lookup"><span data-stu-id="9e98e-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="9e98e-112">O proprietário de um aplicativo não é uma função administrativa.</span><span class="sxs-lookup"><span data-stu-id="9e98e-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="9e98e-113">Se a configuração Restringir o acesso ao portal de administração do [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) estiver habilitada, somente o administrador poderá exibir os aplicativos no portal de Registro de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9e98e-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="9e98e-114">Para que um proprietário possa exibir os aplicativos, desabilite essa configuração (De definir isso como NÃO) ou atribua a função de administrador ao proprietário apenas para o aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="9e98e-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="9e98e-115">No entanto, para isso, você exigirá uma licença do Azure AD Premium P2 e permitirá [o Gerenciamento de Identidade Privilegiada.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="9e98e-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>

---
title: Excluir ou restaurar aplicativos
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013916"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="a98ab-102">Excluir ou restaurar aplicativos</span><span class="sxs-lookup"><span data-stu-id="a98ab-102">Delete or restore applications</span></span>

<span data-ttu-id="a98ab-103">**Para excluir um aplicativo do locatário do Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="a98ab-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="a98ab-104">No **portal do Azure AD,** selecione **aplicativos empresariais.**</span><span class="sxs-lookup"><span data-stu-id="a98ab-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="a98ab-105">Em seguida, encontre e selecione o aplicativo que você deseja excluir.</span><span class="sxs-lookup"><span data-stu-id="a98ab-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="a98ab-106">Na seção **Gerenciar** no painel esquerdo, selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="a98ab-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="a98ab-107">Selecione **Excluir** e, em seguida, **selecione Sim** para confirmar que você deseja excluir o aplicativo do locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a98ab-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="a98ab-108">Para obter mais informações sobre como excluir um aplicativo, consulte Guia de início rápido: excluir um aplicativo do locatário do [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)</span><span class="sxs-lookup"><span data-stu-id="a98ab-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="a98ab-109">No PowerShell, o cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) remove as configurações do Proxy de Aplicativo de um aplicativo específico no Azure Active Directory e pode excluir o aplicativo completamente, se especificado.</span><span class="sxs-lookup"><span data-stu-id="a98ab-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="a98ab-110">Você pode **restaurar um aplicativo excluído usando** o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a98ab-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="a98ab-111">Depois que o aplicativo que você deseja restaurar tiver sido identificado, você poderá restaurá-lo usando [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="a98ab-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>

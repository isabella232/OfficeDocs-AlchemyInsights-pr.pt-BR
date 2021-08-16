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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102559"
---
# <a name="delete-or-restore-applications"></a>Excluir ou restaurar aplicativos

**Para excluir um aplicativo do locatário do Azure AD**:

1. No portal **do Azure AD,** selecione Enterprise **aplicativos**. Em seguida, encontre e selecione o aplicativo que você deseja excluir.
2. Na seção **Gerenciar** no painel esquerdo, selecione **Propriedades**.
3. Selecione **Excluir** e selecione **Sim** para confirmar se deseja excluir o aplicativo do locatário do Azure AD.

Para obter mais informações sobre como excluir um aplicativo, consulte [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

No PowerShell, o cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) remove as configurações de Proxy de Aplicativo de um aplicativo específico no Azure Active Directory e pode excluir o aplicativo completamente, se especificado.

Você pode **restaurar um aplicativo excluído** usando o PowerShell. Depois que o aplicativo que você deseja restaurar tiver sido identificado, você poderá restaurá-lo usando [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).

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
# <a name="delete-or-restore-applications"></a>Excluir ou restaurar aplicativos

**Para excluir um aplicativo do locatário do Azure AD:**

1. No **portal do Azure AD,** selecione **aplicativos empresariais.** Em seguida, encontre e selecione o aplicativo que você deseja excluir.
2. Na seção **Gerenciar** no painel esquerdo, selecione **Propriedades**.
3. Selecione **Excluir** e, em seguida, **selecione Sim** para confirmar que você deseja excluir o aplicativo do locatário do Azure AD.

Para obter mais informações sobre como excluir um aplicativo, consulte Guia de início rápido: excluir um aplicativo do locatário do [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

No PowerShell, o cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) remove as configurações do Proxy de Aplicativo de um aplicativo específico no Azure Active Directory e pode excluir o aplicativo completamente, se especificado.

Você pode **restaurar um aplicativo excluído usando** o PowerShell. Depois que o aplicativo que você deseja restaurar tiver sido identificado, você poderá restaurá-lo usando [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).

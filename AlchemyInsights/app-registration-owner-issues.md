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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951121"
---
# <a name="app-registration-owner-issues"></a>Problemas do Proprietário do Registro de Aplicativos

A seguir estão os métodos disponíveis para adicionar entidades como proprietários para registros de aplicativos:

- Usando o módulo powershell do Azure AD -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referência: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Usando a CLI do Azure - `az ad app owner add`

    Referência: [proprietário do aplicativo do az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Usando o MS Graph -

    Referência: [Adicionar proprietário - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Usando o Portal do Azure AD - Navegue até portal.azure.com [>](https://portal.azure.com/) Azure Active directory > App Registration > Selecione seu aplicativo > Proprietários > Adicionar Proprietários

**Não é possível exibir seu aplicativo na folha Registros de Aplicativos, mesmo que você seja o proprietário desse aplicativo?**

O proprietário de um aplicativo não é uma função administrativa. Se a configuração Restringir o acesso ao portal de administração do [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) estiver habilitada, somente o administrador poderá exibir os aplicativos no portal de Registro de Aplicativos. Para que um proprietário possa exibir os aplicativos, desabilite essa configuração (De definir isso como NÃO) ou atribua a função de administrador ao proprietário apenas para o aplicativo específico. No entanto, para isso, você exigirá uma licença Azure AD Premium P2 e habilitará [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).

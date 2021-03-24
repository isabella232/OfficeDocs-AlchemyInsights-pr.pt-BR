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

O proprietário de um aplicativo não é uma função administrativa. Se a configuração Restringir o acesso ao portal de administração do [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) estiver habilitada, somente o administrador poderá exibir os aplicativos no portal de Registro de Aplicativos. Para que um proprietário possa exibir os aplicativos, desabilite essa configuração (De definir isso como NÃO) ou atribua a função de administrador ao proprietário apenas para o aplicativo específico. No entanto, para isso, você exigirá uma licença do Azure AD Premium P2 e permitirá [o Gerenciamento de Identidade Privilegiada.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)

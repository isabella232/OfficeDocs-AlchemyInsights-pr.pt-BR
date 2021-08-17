---
title: Obter uma lista de Enterprise Aplicativos
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116716"
---
# <a name="get-a-list-of-enterprise-applications"></a>Obter uma lista de Enterprise Aplicativos

1. Para **obter** uma lista de aplicativos corporativos (todos os aplicativos ou filtrados por nome de exibição, ID, URIs de identificador etc.) por meio do comando do Powershell, consulte [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Para obter uma lista de objetos de entidade de serviço (todos os objetos ou filtrados por ID) por meio do comando do Powershell, consulte [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Se você quiser obter uma lista de aplicativos **configurados saml, seguir os scripts do PowerShell** pode ajudá-lo:

    Cada aplicativo seja um aplicativo OAuth ou aplicativo SAML (tanto aplicativos de galeria quanto de não galeria) teria dois objetos criados no AAD quando o registro acontece. Um é chamado de Objeto application e o outro é o objeto Service Principal. Quando você despeja as propriedades de um objeto De entidade de serviço usando o PowerShell, você descobre que cada aplicativo tem um determinado número de Marcas associadas a ele como:

    - Os aplicativos OAuth teriam uma marca chamada "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Galeria SAML Apps teria uma marca chamada "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Aplicativos SAML que não são da Galeria teriam uma marca chamada "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Portanto, você pode usar essas marcas e descobrir que tipo de aplicativo é. A marca "**WindowsAzureActiveDirectoryIntegratedApp**" é comum a todos os tipos de aplicativos. Você pode usar o trecho a seguir para listar todos os aplicativos SAML (galeria e não galeria):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Para obter mais informações, [consulte Identificar aplicativos habilitados para SAML no Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Encontrar e listar somente** aplicativos Web : Use o comando abaixo para obter todos os aplicativos do Azure AD com o tipo de aplicativo "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Encontre e liste aplicativos nativos sozinhos**: Execute o seguinte comando para obter todos os aplicativos nativos de cliente (desktop/dispositivo móvel).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. Exportar todos os detalhes do aplicativo **do Azure AD** registrados para CSV : O comando abaixo exporta todos os aplicativos do Azure AD com detalhes necessários para o arquivo csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Codificação UTF8

7. **Precisa exportar uma lista de aplicativos do Azure** não usados – Relatório de auditoria

    O Azure AD pode mostrar logs de aplicativos por apenas até 30 dias, desde que você tenha Azure AD Premium licença.
    Você tem duas opções para manter os dados por mais de 30 dias. Você pode usar as APIs de Relatório do [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) para recuperar os dados programaticamente e armazená-los em um banco de dados. Como alternativa, você pode integrar logs de auditoria a um sistema SIEM de terceiros.

    Você também pode baixar a lista de aplicativos para todos os aplicativos e aplicativos de propriedade no Azure Active directory>Registros de aplicativos>Baixar>Todos os aplicativos/aplicativos pertencentes.

    Para obter uma lista de aplicativos por meio do MS Graph, consulte Aplicativos de lista [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) e tipo de recurso de aplicativo [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).

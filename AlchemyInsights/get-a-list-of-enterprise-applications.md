---
title: Obter uma lista de Aplicativos Empresariais
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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379770"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="fd437-102">Obter uma lista de Aplicativos Empresariais</span><span class="sxs-lookup"><span data-stu-id="fd437-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="fd437-103">Para **obter** uma lista de aplicativos corporativos (todos os aplicativos ou filtrados por nome de exibição, ID, URIs de identificador etc.) por meio do comando do Powershell, consulte [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="fd437-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="fd437-104">Para obter uma lista de objetos de entidade de serviço (todos os objetos ou filtrados por ID) por meio do comando do Powershell, consulte [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="fd437-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="fd437-105">Se você quiser obter uma lista de aplicativos **configurados saml, seguir os scripts do PowerShell** pode ajudá-lo:</span><span class="sxs-lookup"><span data-stu-id="fd437-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="fd437-106">Cada aplicativo seja um aplicativo OAuth ou aplicativo SAML (tanto aplicativos de galeria quanto de não galeria) teria dois objetos criados no AAD quando o registro acontece.</span><span class="sxs-lookup"><span data-stu-id="fd437-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="fd437-107">Um é chamado de Objeto application e o outro é o objeto Service Principal.</span><span class="sxs-lookup"><span data-stu-id="fd437-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="fd437-108">Quando você despeja as propriedades de um objeto De entidade de serviço usando o PowerShell, você descobre que cada aplicativo tem um determinado número de Marcas associadas a ele como:</span><span class="sxs-lookup"><span data-stu-id="fd437-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="fd437-109">Os aplicativos OAuth teriam uma marca chamada "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="fd437-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="fd437-110">Galeria SAML Apps teria uma marca chamada "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="fd437-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="fd437-111">Aplicativos SAML que não são da Galeria teriam uma marca chamada "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="fd437-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="fd437-112">Portanto, você pode usar essas marcas e descobrir que tipo de aplicativo é.</span><span class="sxs-lookup"><span data-stu-id="fd437-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="fd437-113">A marca "**WindowsAzureActiveDirectoryIntegratedApp**" é comum a todos os tipos de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="fd437-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="fd437-114">Você pode usar o trecho a seguir para listar todos os aplicativos SAML (galeria e não galeria):</span><span class="sxs-lookup"><span data-stu-id="fd437-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="fd437-115">Para obter mais informações, [consulte Identificar aplicativos habilitados para SAML no Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="fd437-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="fd437-116">**Encontrar e listar somente** aplicativos Web : Use o comando abaixo para obter todos os aplicativos do Azure AD com o tipo de aplicativo "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="fd437-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="fd437-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="fd437-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="fd437-118">**Encontre e liste aplicativos nativos sozinhos**: Execute o seguinte comando para obter todos os aplicativos nativos de cliente (desktop/dispositivo móvel).</span><span class="sxs-lookup"><span data-stu-id="fd437-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="fd437-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="fd437-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="fd437-120">Exportar todos os detalhes do aplicativo **do Azure AD** registrados para CSV : O comando abaixo exporta todos os aplicativos do Azure AD com detalhes necessários para o arquivo csv:</span><span class="sxs-lookup"><span data-stu-id="fd437-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="fd437-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="fd437-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="fd437-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Codificação UTF8</span><span class="sxs-lookup"><span data-stu-id="fd437-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="fd437-123">**Precisa exportar uma lista de aplicativos do Azure** não usados – Relatório de auditoria</span><span class="sxs-lookup"><span data-stu-id="fd437-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="fd437-124">O Azure AD pode mostrar logs de aplicativos por apenas até 30 dias, desde que você tenha a licença do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="fd437-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="fd437-125">Você tem duas opções para manter os dados por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="fd437-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="fd437-126">Você pode usar as APIs de Relatório do [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) para recuperar os dados programaticamente e armazená-los em um banco de dados.</span><span class="sxs-lookup"><span data-stu-id="fd437-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="fd437-127">Como alternativa, você pode integrar logs de auditoria a um sistema SIEM de terceiros.</span><span class="sxs-lookup"><span data-stu-id="fd437-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="fd437-128">Você também pode baixar a lista de aplicativos para todos os aplicativos e aplicativos de propriedade no Azure Active directory>Registros de aplicativos>Baixar>Todos os aplicativos/aplicativos pertencentes.</span><span class="sxs-lookup"><span data-stu-id="fd437-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="fd437-129">Para obter uma lista de aplicativos por meio do MS Graph, consulte [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) e application resource type - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="fd437-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>

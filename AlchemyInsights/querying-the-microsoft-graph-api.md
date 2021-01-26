---
title: Consultando a API do Microsoft Graph
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950651"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="605bb-102">Consultando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="605bb-103">Este tópico também pode se aplicar aos desenvolvedores que ainda usam a API do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="605bb-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="605bb-104">No entanto, é **altamente recomendável** que você use o Microsoft Graph para todos os cenários de gerenciamento de diretório, identidade e acesso.</span><span class="sxs-lookup"><span data-stu-id="605bb-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="605bb-105">**Problemas de autenticação ou autorização**</span><span class="sxs-lookup"><span data-stu-id="605bb-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="605bb-106">Se seu aplicativo não conseguir adquirir tokens para chamar o Microsoft Graph, escolha Problema com a aquisição de uma categoria de token de acesso **(Autenticação)** do Microsoft Graph para obter ajuda e suporte mais **específicos** neste tópico.</span><span class="sxs-lookup"><span data-stu-id="605bb-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="605bb-107">Se seu aplicativo estiver recebendo erros de autorização **401 ou 403** ao chamar o Microsoft Graph, escolha a categoria de API do Microsoft Graph obter um erro de acesso negado **(Autorização)** para obter ajuda e suporte mais específicos neste tópico.</span><span class="sxs-lookup"><span data-stu-id="605bb-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="605bb-108">**Quero usar o Microsoft Graph, mas não sei por onde começar**</span><span class="sxs-lookup"><span data-stu-id="605bb-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="605bb-109">Para saber mais sobre o Microsoft Graph, confira:</span><span class="sxs-lookup"><span data-stu-id="605bb-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="605bb-110">Visão geral do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="605bb-111">Visão geral do Gerenciamento de Identidades e Acesso no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="605bb-112">Começar a criar aplicativos do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="605bb-113">**Microsoft Graph Explorer** - Testar as APIs do Microsoft Graph em seu locatário ou em um locatário de demonstração</span><span class="sxs-lookup"><span data-stu-id="605bb-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="605bb-114">**Quero usar o Microsoft Graph, mas ele dá suporte às APIs de diretório v1.0 de que preciso?**</span><span class="sxs-lookup"><span data-stu-id="605bb-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="605bb-115">O Microsoft Graph é a API recomendada para gerenciamento de diretório, identidade e acesso.</span><span class="sxs-lookup"><span data-stu-id="605bb-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="605bb-116">No entanto, ainda há algumas lacunas entre o que é possível no Azure AD Graph e no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="605bb-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="605bb-117">Revise os artigos a seguir, que destacam as diferenças mais atualizadas para ajudar na sua escolha:</span><span class="sxs-lookup"><span data-stu-id="605bb-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="605bb-118">Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="605bb-119">Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="605bb-120">Diferenças de método entre o Azure AD e o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="605bb-121">**Quando eu consulta o *objeto user,* muitas de suas propriedades estão ausentes**</span><span class="sxs-lookup"><span data-stu-id="605bb-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="605bb-122">`GET https://graph.microsoft.com/v1.0/users` retorna apenas 11 propriedades, pois o Microsoft Graph seleciona automaticamente um conjunto padrão de propriedades *do* usuário a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="605bb-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="605bb-123">Se você precisar de outras *propriedades de* usuário, use $select para escolher as propriedades de que seu aplicativo precisa.</span><span class="sxs-lookup"><span data-stu-id="605bb-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="605bb-124">Experimente primeiro no **Microsoft Graph Explorer.**</span><span class="sxs-lookup"><span data-stu-id="605bb-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="605bb-125">**Alguns valores de propriedade do usuário *são nulos,* embora eu saiba que eles estão definidos**</span><span class="sxs-lookup"><span data-stu-id="605bb-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="605bb-126">A explicação mais provável é que o aplicativo tenha sido concedido a *permissão User.ReadBasic.All.*</span><span class="sxs-lookup"><span data-stu-id="605bb-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="605bb-127">Isso permite que o aplicativo leia um conjunto limitado de propriedades do usuário, retornando todas as outras propriedades como nulas, mesmo que elas tenham sido definidas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="605bb-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="605bb-128">Tente conceder ao aplicativo *permissão User.Read.All.*</span><span class="sxs-lookup"><span data-stu-id="605bb-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="605bb-129">Para saber mais, confira [as permissões de usuário do Microsoft Graph.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="605bb-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="605bb-130">**Estou tendo problemas para usar parâmetros de consulta OData para filtrar dados em minhas solicitações**</span><span class="sxs-lookup"><span data-stu-id="605bb-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="605bb-131">Embora o Microsoft Graph suporte a uma ampla variedade de parâmetros de consulta OData, muitos desses parâmetros não são totalmente suportados por serviços de diretório (recursos que herdam de *directoryObject*) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="605bb-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="605bb-132">As mesmas limitações que estavam presentes no Azure AD Graph persistem na maior parte do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="605bb-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="605bb-133">**Sem suporte:**$count, $search e $filter valores *nulos* ou *não nulos*</span><span class="sxs-lookup"><span data-stu-id="605bb-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="605bb-134">**Sem suporte:**$filter em determinadas propriedades (consulte tópicos de recursos nos quais as propriedades são filtáveis)</span><span class="sxs-lookup"><span data-stu-id="605bb-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="605bb-135">**Sem suporte:** paging, filtering e sorting ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="605bb-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="605bb-136">**Sem suporte:** filtrar uma relação.</span><span class="sxs-lookup"><span data-stu-id="605bb-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="605bb-137">Por exemplo: encontre todos os membros do grupo de engenharia que estão no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="605bb-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="605bb-138">**Suporte parcial:**$orderby usuário *(somente* displayName e userPrincipalName) e *grupo*</span><span class="sxs-lookup"><span data-stu-id="605bb-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="605bb-139">**Suporte parcial**: $filter (dá suporte apenas *a eq* *,* *startswith* ou , e *,* e limitado qualquer *)* suporte, $expand (expandir relações de um único objeto retorna todas as relações, mas expandir uma coleção de relações de objetos é limitado)</span><span class="sxs-lookup"><span data-stu-id="605bb-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="605bb-140">Para obter mais informações, [consulte Personalizar respostas com parâmetros de consulta.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="605bb-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="605bb-141">**A API que estou chamando não funciona. Onde posso fazer mais testes?**</span><span class="sxs-lookup"><span data-stu-id="605bb-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="605bb-142">**Microsoft Graph Explorer** - Teste as APIs do Microsoft Graph em seu locatário ou em um locatário de demonstração e também confira as consultas de **exemplo** no Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="605bb-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="605bb-143">**Quando eu consulta dados, parece que estou com um conjunto de dados incompleto definido**</span><span class="sxs-lookup"><span data-stu-id="605bb-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="605bb-144">Se você estiver consultando uma coleção (como *usuários),* o Microsoft Graph usa limites de página do lado do servidor para que os resultados sempre sejam retornados com um tamanho de página padrão.</span><span class="sxs-lookup"><span data-stu-id="605bb-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="605bb-145">Seu aplicativo deve sempre esperar páginas por meio de coleções retornadas do serviço.</span><span class="sxs-lookup"><span data-stu-id="605bb-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="605bb-146">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="605bb-146">For more information, see:</span></span>

- [<span data-ttu-id="605bb-147">Práticas recomendadas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="605bb-148">Paginação de dados do Microsoft Graph em seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="605bb-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="605bb-149">**Meu aplicativo está muito lento e também está sendo diminuído. Quais aprimoramentos posso fazer?**</span><span class="sxs-lookup"><span data-stu-id="605bb-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="605bb-150">Dependendo do seu cenário, há uma variedade de opções diferentes à sua disposição para tornar seu aplicativo mais bem-desempenho e, em alguns casos, menos propenso a ser throttled pelo serviço (quando você está fazendo muitas chamadas).</span><span class="sxs-lookup"><span data-stu-id="605bb-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="605bb-151">Para saber mais, consulte:</span><span class="sxs-lookup"><span data-stu-id="605bb-151">To learn more, see:</span></span>

- [<span data-ttu-id="605bb-152">Práticas recomendadas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="605bb-153">Solicitações de lote</span><span class="sxs-lookup"><span data-stu-id="605bb-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="605bb-154">Controlar alterações por meio da consulta delta</span><span class="sxs-lookup"><span data-stu-id="605bb-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="605bb-155">Ser notificado sobre alterações por meio de webhooks</span><span class="sxs-lookup"><span data-stu-id="605bb-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="605bb-156">Diretrizes de throttling</span><span class="sxs-lookup"><span data-stu-id="605bb-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="605bb-157">**Onde posso encontrar mais informações sobre erros e problemas conhecidos?**</span><span class="sxs-lookup"><span data-stu-id="605bb-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="605bb-158">Informações de resposta a erros do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="605bb-159">Problemas conhecidos com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="605bb-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="605bb-160">**Onde posso verificar o status de disponibilidade e conectividade do serviço?**</span><span class="sxs-lookup"><span data-stu-id="605bb-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="605bb-161">A disponibilidade do serviço e a conectividade dos serviços subjacentes que podem ser acessados por meio do Microsoft Graph podem afetar a disponibilidade e o desempenho gerais do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="605bb-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="605bb-162">Para a saúde do serviço do Azure Active Directory, verifique o status dos serviços de Segurança **+** Identidade listados na página [de status do Azure.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="605bb-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="605bb-163">Para serviços do Office que contribuem para o Microsoft Graph, verifique o status dos serviços listados no Painel [de Saúde do Serviço do Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="605bb-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

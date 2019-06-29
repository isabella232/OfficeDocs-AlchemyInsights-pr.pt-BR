---
title: O conteúdo não aparece nos resultados de pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363785"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="84d07-102">O conteúdo não aparece nos resultados de pesquisa do SharePoint</span><span class="sxs-lookup"><span data-stu-id="84d07-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="84d07-103">Siga estas etapas de solução de problemas quando o conteúdo esperado não aparecer nos resultados da pesquisa:</span><span class="sxs-lookup"><span data-stu-id="84d07-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="84d07-104">Verifique se o **site** que contém o conteúdo esperado está definido para permitir que o conteúdo apareça nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="84d07-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="84d07-105">Siga as etapas em [Mostrar conteúdo em um site nos resultados da pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="84d07-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="84d07-106">Verifique se a **lista** ou **biblioteca** que contém o conteúdo esperado está definida para permitir que o conteúdo apareça nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="84d07-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="84d07-107">Siga as etapas em [Mostrar conteúdo de listas ou bibliotecas nos resultados da pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="84d07-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="84d07-108">Verifique se o layout de página, documento ou página personalizada está publicado como uma **versão principal.**</span><span class="sxs-lookup"><span data-stu-id="84d07-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="84d07-109">Siga a etapa 3 na [pesquisa não retorna todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="84d07-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="84d07-110">Verifique se o usuário tem **permissões** para exibir o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="84d07-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="84d07-111">Siga as etapas na [compreensão dos níveis de permissão no SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="84d07-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="84d07-112">Se o esquema de pesquisa tiver sido alterado adicionando uma nova propriedade gerenciada, editando uma propriedade gerenciada ou removendo uma propriedade gerenciada, solicitando um rastreamento e um novo índice será necessário.</span><span class="sxs-lookup"><span data-stu-id="84d07-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="84d07-113">**Indexe novamente** o conteúdo seguindo as etapas em [solicitar manualmente o rastreamento e a reindexação de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="84d07-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="84d07-114">Isso pode levar algum tempo, aguardar 24 horas antes de verificar os resultados novamente.</span><span class="sxs-lookup"><span data-stu-id="84d07-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="84d07-115">Para obter mais informações, consulte [habilitar o conteúdo em um site a ser pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="84d07-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  

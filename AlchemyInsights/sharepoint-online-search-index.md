---
title: Gerenciar dicionários de pesquisa no SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736041"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="f5bed-102">Pesquisa no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f5bed-102">Search in SharePoint Online</span></span>

<span data-ttu-id="f5bed-103">O conteúdo deve ser rastreado e adicionado ao índice de pesquisa para que os usuários encontrem o que estão procurando no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f5bed-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="f5bed-104">O conteúdo é rastreado automaticamente com base em um cronograma de rastreamento predefinido (o cronograma de rastreamento não pode ser alterado).</span><span class="sxs-lookup"><span data-stu-id="f5bed-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="f5bed-105">O rastreador seleciona o conteúdo que foi alterado desde o último rastreamento e atualiza o índice.</span><span class="sxs-lookup"><span data-stu-id="f5bed-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="f5bed-106">Para garantir que o conteúdo seja rastreado e o índice seja atualizado, siga as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="f5bed-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="f5bed-107">Certifique-se de que o conteúdo pode ser encontrado ao tornar o conteúdo do site pesquisável.</span><span class="sxs-lookup"><span data-stu-id="f5bed-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="f5bed-108">Para saber mais, confira [habilitar o conteúdo em um site que poderá ser pesquisado](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="f5bed-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="f5bed-109">Quando você tiver alterado uma propriedade gerenciada ou quando tiver alterado o mapeamento de propriedades rastreadas e gerenciadas, o site deverá ser rastreado novamente para que as alterações sejam refletidas no índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f5bed-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="f5bed-110">Como as alterações são feitas no esquema de pesquisa e não no site real, o rastreador não irá indexar automaticamente o site.</span><span class="sxs-lookup"><span data-stu-id="f5bed-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="f5bed-111">Para saber mais, confira [solicitar o rastreamento e a reindexação de um site, uma biblioteca ou uma lista manualmente](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="f5bed-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="f5bed-112">Aguarde pelo menos 24 horas depois de solicitar manualmente um rastreamento e um novo índice completo para ver se ainda está ocorrendo um problema.</span><span class="sxs-lookup"><span data-stu-id="f5bed-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="f5bed-113">Se passar mais de 24 horas desde que você iniciou o rastreamento e o REINDEX completo, registre um caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="f5bed-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="f5bed-114">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="f5bed-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f5bed-115">Aguarde pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="f5bed-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="f5bed-116">**Importante**: se um site, documento (biblioteca) ou uma lista tiver sido excluído e ainda for exibido nos resultados da pesquisa, os usuários deverão receber um erro 404 arquivo não encontrado ao tentar acessar.</span><span class="sxs-lookup"><span data-stu-id="f5bed-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="f5bed-117">Esse problema deve ser registrado como um caso de suporte para uma investigação adicional.</span><span class="sxs-lookup"><span data-stu-id="f5bed-117">This issue should be logged as a support case for further investigation.</span></span> 




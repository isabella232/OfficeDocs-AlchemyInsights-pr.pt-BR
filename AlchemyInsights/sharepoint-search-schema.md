---
title: Gerenciar o esquema de pesquisa no SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270084"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="7b11e-102">Gerenciar o esquema de pesquisa no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7b11e-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="7b11e-103">O esquema de pesquisa controla o que os usuários podem pesquisar, como os usuários podem procurá-lo e como você pode apresentar os resultados nos seus sites de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7b11e-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="7b11e-104">Consulte [gerenciar o esquema de pesquisa no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) para saber como:</span><span class="sxs-lookup"><span data-stu-id="7b11e-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="7b11e-105">Alterar o esquema de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7b11e-105">Change the search schema.</span></span>
- <span data-ttu-id="7b11e-106">Criar propriedades gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="7b11e-106">Create managed properties.</span></span>
- <span data-ttu-id="7b11e-107">Mapear propriedades rastreadas do mapa rastreado para propriedades gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="7b11e-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="7b11e-108">Observe o seguinte em relação ao gerenciamento do esquema de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="7b11e-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="7b11e-109">Se você receber um aviso informando que **o aplicativo está pausado** quando fizer uma alteração no esquema, isso só será temporário, pois ocorrerá manutenção do serviço.</span><span class="sxs-lookup"><span data-stu-id="7b11e-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="7b11e-110">Se tiver passado mais de 24 horas e você ainda tiver o aviso, registre um caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="7b11e-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="7b11e-111">Quando você alterar as propriedades gerenciadas ou adicionar novas, as alterações terão efeito somente depois que o conteúdo for rastreado novamente.</span><span class="sxs-lookup"><span data-stu-id="7b11e-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="7b11e-112">No SharePoint Online, o rastreamento ocorre automaticamente com base no cronograma de rastreamento definido.</span><span class="sxs-lookup"><span data-stu-id="7b11e-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="7b11e-113">Para garantir que suas alterações sejam rastreadas, você pode solicitar especificamente [uma reindexação da lista ou biblioteca](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="7b11e-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="7b11e-114">Para obter uma visão geral completa do esquema de pesquisa, consulte [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="7b11e-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 



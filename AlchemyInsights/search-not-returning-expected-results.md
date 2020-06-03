---
title: 1491-pesquisa-não-retorno-esperado-resultados
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510560"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="dde47-102">A pesquisa de conteúdo não retorna os resultados esperados</span><span class="sxs-lookup"><span data-stu-id="dde47-102">Content Search not returning expected results</span></span>

<span data-ttu-id="dde47-103">Ao executar conteúdo pesquisa a partir do centro de conformidade & segurança da Microsoft 365, você pode receber resultados de pesquisa inesperados.</span><span class="sxs-lookup"><span data-stu-id="dde47-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="dde47-104">Considere as seguintes coisas que podem afetar seus resultados de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="dde47-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="dde47-105">**Locais e condições de pesquisa de conteúdo**: Certifique-se de ter selecionado os locais de conteúdo e as condições de pesquisa apropriados.</span><span class="sxs-lookup"><span data-stu-id="dde47-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="dde47-106">Se você executou uma pesquisa grande (com muitos locais), considere dividi-la em várias pesquisas.</span><span class="sxs-lookup"><span data-stu-id="dde47-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="dde47-107">**Itens parcialmente indexados**: [itens parcialmente indexados](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) de caixas de correio são incluídos nos resultados estimados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="dde47-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="dde47-108">No entanto, itens parcialmente indexados de sites no SharePoint e no OneDrive não estão incluídos na estimativa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="dde47-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="dde47-109">**Falhas de pesquisa**: ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), você pode receber erros de pesquisa, com códigos de erro como CS008-009 e CS012-002).</span><span class="sxs-lookup"><span data-stu-id="dde47-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="dde47-110">Nesse caso, repita a pesquisa para os locais de conteúdo com falha.</span><span class="sxs-lookup"><span data-stu-id="dde47-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="dde47-111">Confira [Este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="dde47-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

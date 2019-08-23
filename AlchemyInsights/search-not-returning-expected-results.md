---
title: 1491-pesquisa-não-retorno-esperado-resultados
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551403"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="e1f28-102">A pesquisa de conteúdo não retorna os resultados esperados</span><span class="sxs-lookup"><span data-stu-id="e1f28-102">Content Search not returning expected results</span></span>

<span data-ttu-id="e1f28-103">Ao executar conteúdo pesquisa a partir do centro de conformidade & segurança do Office 365, você pode receber resultados de pesquisa inesperados.</span><span class="sxs-lookup"><span data-stu-id="e1f28-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="e1f28-104">Considere as seguintes coisas que podem afetar seus resultados de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="e1f28-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="e1f28-105">**Locais e condições de pesquisa de conteúdo**: Certifique-se de ter selecionado os locais de conteúdo e as condições de pesquisa apropriados.</span><span class="sxs-lookup"><span data-stu-id="e1f28-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="e1f28-106">Se você executou uma pesquisa grande (com muitos locais), considere dividi-la em várias pesquisas.</span><span class="sxs-lookup"><span data-stu-id="e1f28-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="e1f28-107">**Itens parcialmente indexados**: [itens parcialmente indexados](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) de caixas de correio são incluídos nos resultados estimados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e1f28-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="e1f28-108">No entanto, itens parcialmente indexados de sites no SharePoint e no OneDrive não estão incluídos na estimativa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e1f28-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="e1f28-109">**Falhas de pesquisa**: ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), você pode receber erros de pesquisa, com códigos de erro como CS008-009 e CS012-002).</span><span class="sxs-lookup"><span data-stu-id="e1f28-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="e1f28-110">Nesse caso, repita a pesquisa para os locais de conteúdo com falha.</span><span class="sxs-lookup"><span data-stu-id="e1f28-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="e1f28-111">Confira [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e1f28-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>

---
title: 1491-Search-not-Returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964797"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="2459e-102">Pesquisa de conteúdo que não retorne os resultados esperados</span><span class="sxs-lookup"><span data-stu-id="2459e-102">Content Search not returning expected results</span></span>

<span data-ttu-id="2459e-p101">Ao executar pesquisas de conteúdo a partir do Centro de conformidade do & de segurança do Office 365, você pode receber resultados inesperados de pesquisa. Considere os seguintes itens que podem afetar os resultados de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="2459e-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="2459e-p102">**Locais de conteúdo e condições de pesquisa**: Verifique se você selecionou os locais de conteúdo adequados e critérios de pesquisa. Se você executou uma pesquisa de grande porte (com muitos locais), considere dividindo-lo em várias pesquisas.</span><span class="sxs-lookup"><span data-stu-id="2459e-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="2459e-p103">**Itens de indexados parcialmente**: [parcialmente indexados itens](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas postais estão incluídos nos resultados da pesquisa estimados. No entanto, itens parcialmente indexados de sites no SharePoint e OneDrive não estão incluídos na estimativa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2459e-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="2459e-p104">**Falhas de pesquisa**: ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), você poderá obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Nesse caso, repita a pesquisa somente para os locais de conteúdo com falha. Consulte [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="2459e-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>

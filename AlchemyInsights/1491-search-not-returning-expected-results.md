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
# <a name="content-search-not-returning-expected-results"></a>Pesquisa de conteúdo que não retorne os resultados esperados

Ao executar pesquisas de conteúdo a partir do Centro de conformidade do & de segurança do Office 365, você pode receber resultados inesperados de pesquisa. Considere os seguintes itens que podem afetar os resultados de pesquisa:

- **Locais de conteúdo e condições de pesquisa**: Verifique se você selecionou os locais de conteúdo adequados e critérios de pesquisa. Se você executou uma pesquisa de grande porte (com muitos locais), considere dividindo-lo em várias pesquisas.

- **Itens de indexados parcialmente**: [parcialmente indexados itens](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas postais estão incluídos nos resultados da pesquisa estimados. No entanto, itens parcialmente indexados de sites no SharePoint e OneDrive não estão incluídos na estimativa de pesquisa.

- **Falhas de pesquisa**: ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), você poderá obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Nesse caso, repita a pesquisa somente para os locais de conteúdo com falha. Consulte [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.

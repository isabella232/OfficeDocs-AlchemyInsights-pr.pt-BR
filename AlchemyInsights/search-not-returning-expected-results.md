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
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709215"
---
# <a name="content-search-not-returning-expected-results"></a>A pesquisa de conteúdo não retorna os resultados esperados

Ao executar conteúdo pesquisa a partir do centro de conformidade & segurança da Microsoft 365, você pode receber resultados de pesquisa inesperados. Considere as seguintes coisas que podem afetar seus resultados de pesquisa:

- **Locais e condições de pesquisa de conteúdo**: Certifique-se de ter selecionado os locais de conteúdo e as condições de pesquisa apropriados. Se você executou uma pesquisa grande (com muitos locais), considere dividi-la em várias pesquisas.

- **Itens parcialmente indexados**: [itens parcialmente indexados](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) de caixas de correio são incluídos nos resultados estimados da pesquisa. No entanto, itens parcialmente indexados de sites no SharePoint e no OneDrive não estão incluídos na estimativa de pesquisa.

- **Falhas de pesquisa**: ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), você pode receber erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Nesse caso, repita a pesquisa para os locais de conteúdo com falha. Confira [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.

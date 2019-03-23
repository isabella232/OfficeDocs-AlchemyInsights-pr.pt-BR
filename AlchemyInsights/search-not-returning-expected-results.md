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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776070"
---
# <a name="content-search-not-returning-expected-results"></a>A pesquisa de conteúdo não retorna os resultados esperados

Ao executar conteúdo pesquisa do centro de conformidade do & de segurança do Office 365, você pode receber resultados de pesquisa inesperados. Considere as seguintes coisas que podem afetar seus resultados de pesquisa:

- **Locais e condições de pesquisa de conteúdo**: Certifique-se de ter selecionado os locais de conteúdo e as condições de pesquisa apropriados. Se você executou uma pesquisa grande (com muitos locais), considere dividi-la em várias pesquisas.

- **Itens parcialmente indexados**: [itens parcialmente indexados](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) de caixas de correio são incluídos nos resultados estimados da pesquisa. No enTanto, itens parcialmente indexados de sites no SharePoint e no OneDrive não estão incluídos na estimativa de pesquisa.

- **Falhas de pesquisa**: ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), você pode receber erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Nesse caso, repita a pesquisa para os locais de conteúdo com falha. ConFira [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.

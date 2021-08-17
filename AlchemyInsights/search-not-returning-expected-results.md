---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052698"
---
# <a name="content-search-not-returning-expected-results"></a>Pesquisa de Conteúdo não retornando resultados esperados

Ao executar pesquisas de conteúdo no centro de conformidade Microsoft 365 segurança & segurança, você pode receber resultados inesperados de pesquisa. Considere as seguintes coisas que podem afetar seus resultados de pesquisa:

- **Locais de conteúdo e condições de pesquisa:** certifique-se de ter selecionado os locais de conteúdo e as condições de pesquisa adequadas. Se você realizou uma pesquisa grande (com muitos locais), considere dividi-la em várias pesquisas.

- **Itens parcialmente indexados:**  [Itens parcialmente indexados](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) de caixas de correio são incluídos nos resultados estimados da pesquisa. No entanto, itens parcialmente indexados de sites SharePoint e OneDrive não estão incluídos na estimativa de pesquisa.

- **Falhas de** pesquisa : ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), você pode obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Nesse caso, repetir a pesquisa somente para os locais de conteúdo com falha. Confira  [este artigo para](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) obter mais informações.

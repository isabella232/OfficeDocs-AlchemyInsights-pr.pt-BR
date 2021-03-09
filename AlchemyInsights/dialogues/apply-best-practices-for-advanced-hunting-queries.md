---
title: Aplicar práticas recomendadas para consultas avançadas de busca
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568446"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="c73df-102">Aplicar práticas recomendadas para consultas avançadas de busca</span><span class="sxs-lookup"><span data-stu-id="c73df-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="c73df-103">Para obter resultados mais rápidos e evitar tempo-de-tempo durante a execução de consultas complexas, aplique estas práticas recomendadas:</span><span class="sxs-lookup"><span data-stu-id="c73df-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="c73df-104">Ao tentar novas consultas, sempre use um limite para evitar obter conjuntos de resultados extremamente grandes.</span><span class="sxs-lookup"><span data-stu-id="c73df-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="c73df-105">Além disso, `count` use para fazer uma avaliação inicial do tamanho do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c73df-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="c73df-106">Use primeiro os filtros de tempo.</span><span class="sxs-lookup"><span data-stu-id="c73df-106">Use time filters first.</span></span> <span data-ttu-id="c73df-107">O ideal é limitar suas consultas a sete dias.</span><span class="sxs-lookup"><span data-stu-id="c73df-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="c73df-108">No início de uma consulta, logo após o filtro de hora, adicione os filtros esperados para remover a maioria dos dados.</span><span class="sxs-lookup"><span data-stu-id="c73df-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="c73df-109">Ao procurar tokens completos, use o `has` operador em vez de `contains` .</span><span class="sxs-lookup"><span data-stu-id="c73df-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="c73df-110">Execute uma pesquisa em uma coluna específica, em vez de em todas as colunas.</span><span class="sxs-lookup"><span data-stu-id="c73df-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="c73df-111">Ao ingressar em tabelas, primeiro especifique a tabela com menos linhas.</span><span class="sxs-lookup"><span data-stu-id="c73df-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="c73df-112">`project` somente as colunas necessárias das tabelas que você ingressou.</span><span class="sxs-lookup"><span data-stu-id="c73df-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="c73df-113">Para saber mais, confira [Práticas recomendadas de consulta de busca avançada.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="c73df-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>

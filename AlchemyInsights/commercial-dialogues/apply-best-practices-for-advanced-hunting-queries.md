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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930121"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Aplicar práticas recomendadas para consultas avançadas de busca

Para obter resultados mais rápidos e evitar tempo-de-tempo durante a execução de consultas complexas, aplique estas práticas recomendadas:

- Ao tentar novas consultas, sempre use um limite para evitar obter conjuntos de resultados extremamente grandes. Além disso, `count` use para fazer uma avaliação inicial do tamanho do conjunto de resultados.
- Use primeiro os filtros de tempo. O ideal é limitar suas consultas a sete dias.
- No início de uma consulta, logo após o filtro de hora, adicione os filtros esperados para remover a maioria dos dados.
- Ao procurar tokens completos, use o `has` operador em vez de `contains` .
- Execute uma pesquisa em uma coluna específica, em vez de em todas as colunas.
- Ao ingressar em tabelas, primeiro especifique a tabela com menos linhas.
- `project` somente as colunas necessárias das tabelas que você ingressou.

Para saber mais, confira [Práticas recomendadas de consulta de busca avançada.](https://go.microsoft.com/fwlink/?linkid=2144812)

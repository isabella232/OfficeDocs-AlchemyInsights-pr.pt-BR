---
title: Gráfico mostra um número diferente de registros na grade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793746"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Gráfico mostra um número diferente de registros na grade

**Sintoma**

Em um gráfico no página de painel, quando clicar no gráfico "..." e clicar em "Exibir registros", navegue até a página de grade para ver todos os registros. Às vezes, o número de registros é alterado.

**Causa**

Isso ocorre devido à diferença de modos de exibição entre o gráfico na página de painel original e o gráfico na página inicial da grade.  

**Solução**

1. Verifique o modo de exibição da página original e o modo de exibição da grade para ver se eles são diferentes.
2. Altere o modo de exibição da grade para corresponder ao modo de exibição na página original.
3. Se não for possível encontrar o modo de exibição correto, isso significa que o modo de exibição não está habilitado no designer de aplicativo.
4. Vá para o designer de aplicativo do aplicativo específico, escolha a entidade e seus modos de exibição, verifique o modo de exibição que você deseja habilitar, salvar, publicar e feche.
5. Atualize a página.
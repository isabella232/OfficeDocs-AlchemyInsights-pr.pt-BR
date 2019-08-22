---
title: O conteúdo não aparece nos resultados de pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517019"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>O conteúdo não aparece nos resultados de pesquisa do SharePoint

Siga estas etapas de solução de problemas quando o conteúdo esperado não aparecer nos resultados da pesquisa:
  
1. Verifique se o **site** que contém o conteúdo esperado está definido para permitir que o conteúdo apareça nos resultados da pesquisa. Siga as etapas em [Mostrar conteúdo em um site nos resultados da pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verifique se a **lista** ou **biblioteca** que contém o conteúdo esperado está definida para permitir que o conteúdo apareça nos resultados da pesquisa. Siga as etapas em [Mostrar conteúdo de listas ou bibliotecas nos resultados da pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verifique se o layout de página, documento ou página personalizada está publicado como uma **versão principal.** Siga a etapa 3 na [pesquisa não retorna todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verifique se o usuário tem **permissões** para exibir o conteúdo. Siga as etapas na [compreensão dos níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Se o esquema de pesquisa tiver sido alterado adicionando uma nova propriedade gerenciada, editando uma propriedade gerenciada ou removendo uma propriedade gerenciada, solicitando um rastreamento e um novo índice será necessário. **Indexe novamente** o conteúdo seguindo as etapas em [solicitar manualmente o rastreamento e a reindexação de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Isso pode levar algum tempo, aguardar 24 horas antes de verificar os resultados novamente.

Para obter mais informações, consulte [habilitar o conteúdo em um site a ser pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  

---
title: Pesquisa no SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507619"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Rastreamento e indexação de conteúdo no SharePoint Online

O conteúdo deve ser rastreado e adicionado ao índice de pesquisa para que os usuários encontrem o que estão procurando no SharePoint Online. O conteúdo é rastreado automaticamente com base em um cronograma de rastreamento predefinido (o cronograma de rastreamento não pode ser alterado). O rastreador seleciona o conteúdo que foi alterado desde o último rastreamento e atualiza o índice. Para garantir que o conteúdo seja rastreado e o índice seja atualizado, observe o seguinte:

- Certifique-se de que o conteúdo pode ser encontrado ao [tornar o conteúdo do site pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Quando você tiver alterado uma propriedade gerenciada ou quando tiver alterado o mapeamento de propriedades rastreadas e gerenciadas, o site deverá ser rastreado novamente para que as alterações sejam refletidas no índice de pesquisa. 

    Como as alterações são feitas no esquema de pesquisa e não no site real, o rastreador não irá indexar automaticamente o site. 

    Para saber mais, confira [solicitar o rastreamento e a reindexação de um site, uma biblioteca ou uma lista manualmente](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Aguarde pelo menos 24 horas depois de solicitar manualmente um rastreamento e um novo índice completo para ver se ainda está ocorrendo um problema. 

    Se passar mais de 24 horas desde que você iniciou o rastreamento e o REINDEX completo, registre um caso de suporte. Em muitos casos, já estamos trabalhando em uma solução. Aguarde pelo menos 24 horas para concluir uma solução.

> [!IMPORTANT]
> Se um site, documento (biblioteca) ou uma lista tiver sido excluído e ainda for exibido nos resultados da pesquisa, os usuários deverão receber um **erro 404 arquivo não encontrado** ao tentar acessá-lo. Esse problema deve ser registrado como um caso de suporte para uma investigação adicional. 




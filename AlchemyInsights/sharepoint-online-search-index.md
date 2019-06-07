---
title: Gerenciar dicionários de pesquisa no SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758754"
---
# <a name="search-in-sharepoint-online"></a>Pesquisa no SharePoint Online

O conteúdo deve ser rastreado e adicionado ao índice de pesquisa para que os usuários encontrem o que estão procurando no SharePoint Online. O conteúdo é rastreado automaticamente com base em um cronograma de rastreamento predefinido (o cronograma de rastreamento não pode ser alterado). O rastreador seleciona o conteúdo que foi alterado desde o último rastreamento e atualiza o índice. Para garantir que o conteúdo seja rastreado e o índice seja atualizado, siga as etapas abaixo.

Certifique-se de que o conteúdo pode ser encontrado ao tornar o conteúdo do site pesquisável. Para saber mais, confira [habilitar o conteúdo em um site que poderá ser pesquisado](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

Quando você tiver alterado uma propriedade gerenciada ou quando tiver alterado o mapeamento de propriedades rastreadas e gerenciadas, o site deverá ser rastreado novamente para que as alterações sejam refletidas no índice de pesquisa. 

Como as alterações são feitas no esquema de pesquisa e não no site real, o rastreador não irá indexar automaticamente o site. 

Para saber mais, confira [solicitar o rastreamento e a reindexação de um site, uma biblioteca ou uma lista manualmente](https://docs.microsoft.com/sharepoint/crawl-site-conten).

 Aguarde pelo menos 24 horas depois de solicitar manualmente um rastreamento e um novo índice completo para ver se ainda está ocorrendo um problema. 

Se passar mais de 24 horas desde que você iniciou o rastreamento e o REINDEX completo, registre um caso de suporte. Em muitos casos, já estamos trabalhando em uma solução. Aguarde pelo menos 24 horas para concluir uma solução.

**Importante**: se um site, documento (biblioteca) ou uma lista tiver sido excluído e ainda for exibido nos resultados da pesquisa, os usuários deverão receber um erro 404 arquivo não encontrado ao tentar acessar. Esse problema deve ser registrado como um caso de suporte para uma investigação adicional. 




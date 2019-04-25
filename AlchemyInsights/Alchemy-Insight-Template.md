---
title: igual ao nome do arquivo é melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366319"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Cabeçalho Alchemy necessário H1, H2's não funcionam.
Práticas recomendadas e diretrizes para a criação de Alchemy:

1. **Não aninhe Alchemy insights em Folders**: isso quebrará a estrutura da URL. Estamos tentando corrigir isso.
1. Os arquivos na pasta **AlchemyInsights** devem ter nomes de arquivo em minúsculas com hifens para espaços por exemplo. ***How-to-Enable-litígio-Hold***.
    1. Inclua a ID de regra ou a ID de Bucket do [portal do parceiro Alchemy](https://alchemyportal.azurewebsites.net) no campo MS. Custom. ex. ***MS. Custom: 100021***
1. Use o restante dos metadados na parte superior do arquivo como modelo.
1. No [portal do parceiro do Alchemy](https://alchemyportal.azurewebsites.net), navegue até a seção **título do atendimento ao cliente:** e use-o como ponto de partida para o título H1 da visão. 
    > [!NOTE]
    > O Alchemy insights deve ter apenas um único H1 na parte superior ou eles serão quebrados na produção. H2S não renderizar use **negrito** ou outras convenções para indicar seções separadas.
1. Em seguida, preencha o corpo de texto usando o material de rascunho na seção do cliente ideias da página de regra Alchemy
    1. Listas com marcadores são boas
    1. Listas numeradas muito
    1. **Negrito** e *itálico* são a-ok
    1. Os links devem ser sempre **"links para a Web"/External** ou **links de profundidade para elementos da interface do usuário**, não para links internos.
    1. As imagens não são oficialmente suportadas no momento, mas estão no roteiro.

E isso já é um pouco longo demais. A prática recomendada é de cerca de 400 caracteres---------------------------------

Depois que o conteúdo estiver pronto, puxe-o para o Live Branch. Em seguida, vá para o [portal do parceiro Alchemy](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo URL. M
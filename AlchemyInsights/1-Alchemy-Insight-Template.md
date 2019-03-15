---
title: 'igual ao nome do arquivo é melhor [regra #-Descrição]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634492"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Cabeçalho Alchemy necessário H1, H2's não funcionam.
Práticas recomendadas e diretrizes para a criação de Alchemy:

1. **Não aninhe Alchemy insights em Folders**: isso quebrará a estrutura da URL. Estamos tentando corrigir isso.
1. Os arquivos na pasta **AlchemyInsights** devem ter ID de regra e nome de regra do [portal de parceiro do Alchemy](https://alchemyportal.azurewebsites.net) no nome do arquivo.
    1. ex. ***976-instruções-Enable-litígio-retenção***
1. Use os metadados na parte superior desse arquivo como modelo. Nada mais é necessário.
1. No [portal do parceiro do Alchemy](https://alchemyportal.azurewebsites.net), navegue até a seção **título do atendimento ao cliente:** e use-o como ponto de partida para o título H1 da visão. 
    > [!NOTE]
    > O Alchemy insights deve ter apenas um único H1 na parte superior ou eles serão quebrados na produção. H2S não renderizar use **negrito** ou outras convenções para indicar seções separadas.
1. Em seguida, preencha o corpo de texto usando o material de rascunho na seção do cliente ideias da página de regra Alchemy
    1. Listas com marcadores são boas
    1. Listas numeradas muito
    1. **Negrito** e *itálico* são a-ok
    1. Os links devem ser sempre **"links para a Web"/External** ou **links de profundidade para elementos da interface do usuário**, não para links internos.

E isso já é um pouco longo demais. A prática recomendada é de cerca de 400 caracteres---------------------------------

Depois que o conteúdo estiver pronto, puxe-o para o Live Branch. Em seguida, vá para o [portal do parceiro Alchemy](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo URL. Verifique se as informações revisadas e publicadas diz "Sim" e clique em atualizar regra. **(Isso será prettier na nova versão do portal-lançamento em breve.)** 
 ![campo URL](media/for-content-team.PNG)


---
title: 'é igual ao nome de arquivo é melhor [regra #-descrição]'
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
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939265"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obrigatório Alquimia cabeçalho S1, S2 não funcionam.
Práticas recomendadas e diretrizes para a criação de Alquimia:

1. **Não aninhar Alquimia ideias de pesquisas nas pastas**- Isso interromperá a estrutura da url. Estamos analisando corrigindo isso.
1. Arquivos na pasta **AlchemyInsights** devem ter o ID da regra e o nome da regra a partir do [portal Alquimia parceiro](https://alchemyportal.azurewebsites.net) no nome de arquivo.
    1. ***976-How-to-enable-litigation-hold*** ex.
1. Use os metadados na parte superior desse arquivo como seu modelo. Nada mais é necessário.
1. No [portal Alquimia parceiro](https://alchemyportal.azurewebsites.net), navegue até a seção **título percepção de cliente:** e usá-la como uma partida aponte para seu título S1 para o insight. 
    > [!NOTE]
    > Ideias de Alquimia deve ter apenas um único S1 na parte superior ou eles serão interrompidos em produção. H2s não processar afirmativo usar **negrito** ou outras convenções para significar seções separadas.
1. Em seguida, preencha o corpo de texto usando o material de rascunho na seção ideias dos clientes da página Alquimia regra
    1. Listas com marcadores são finas
    1. Muito de listas numeradas
    1. **Negrito** e *itálico* são a-ok
    1. Links sempre deve ser um **"links web" / externo** OR **profunda-links para os elementos de interface do usuário**, os links não internos.

E isso realmente já é um pouco muito longo. Prática recomendada é aproximadamente 400 caracteres--

Depois que o conteúdo está pronto, retire-o à ramificação ao vivo. Em seguida, vá para o [portal de parceiros Alquimia](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo url. Certifique-se de Insight revisado e publicado diz "Sim" e clique em regra de atualização. **(Isso terá uma aparência mais bonito na nova versão do portal - liberando em breve.)** 
 ![campo url](media/for-content-team.PNG)


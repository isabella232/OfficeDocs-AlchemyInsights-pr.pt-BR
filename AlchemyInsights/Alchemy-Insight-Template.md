---
title: mesmo que filename seja o melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312813"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"O Header de Alquimia necessário H1, H2 não funciona."
Práticas recomendadas e diretrizes para a autoria de Alquimia:

1. **Não aninhar alquimia Insights em pastas**- isso quebrará a estrutura da URL. Estamos tentando corrigir isso.
1. Os arquivos na **pasta AlchemyInsights** devem ter nomes de arquivo minúsculos com hífens para espaços ex. **_how-to-enable-litigation-hold_**.
    1. Inclua a ID de regra ou a ID do bucket do portal do [Parceiro de Alquimia](https://alchemyportal.azurewebsites.net) no campo ms.custom. ex. ***ms.custom: 100021***
1. Use o restante dos metadados na parte superior deste arquivo como seu modelo.
1. No [portal do Parceiro de Alquimia,](https://alchemyportal.azurewebsites.net)navegue até a seção **Customer Insight Title:** e use-o como ponto de partida para o título H1 para o insight. 

**Observação**: a Insights deve ter apenas um único H1 na parte superior ou eles quebrarão na produção. H2s não renderiza, portanto, use **negrito** ou outras convenções para significar seções separadas.
1. Em seguida, preencha o texto do corpo usando o material de rascunho na seção Customer Insights da página Regra de Alquimia
    1. Listas com marcador estão ótimas
    1. Listas numeradas também
    1. **Negrito** *e itálico* são a-ok
    1. Os links sempre devem ser **"links para a Web"/links** **profundos** ou externos para elementos da interface do usuário, não links internos.
    1. As imagens não têm suporte oficial no momento, mas estão no roteiro.

E isso já é um pouco longo demais. A prática prática é de cerca de 400 caracteres ---------------------------------

Depois que o conteúdo estiver pronto, puxe-o para a ramificação ao vivo. Em seguida, vá para o portal do Parceiro [de Alquimia](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo url. 
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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918880"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"O Header de Alquimia necessário H1, H2 não funciona."
Práticas recomendadas e diretrizes para a autoria de Alquimia:

1. **Não aninhar alquimia Insights em pastas**- isso quebrará a estrutura da URL. Estamos tentando corrigir isso.
1. Os arquivos na **pasta AlchemyInsights** devem ter nomes de arquivo minúsculos com hífens para espaços ex. **_how-to-enable-litigation-hold_**.
    1. Inclua a ID de regra ou a ID do bucket do portal do [Parceiro de Alquimia](https://alchemyportal.azurewebsites.net) no campo ms.custom. ex. ***ms.custom: 100021***
1. Use o restante dos metadados na parte superior deste arquivo como seu modelo.
1. No [portal do Parceiro de Alquimia,](https://alchemyportal.azurewebsites.net)navegue até a seção **Customer Insight Title:** e use-o como ponto de partida para o título H1 para o insight. 
    > [!NOTE]
    > A Insights alquimia deve ter apenas um único H1 na parte superior ou eles quebrarão na produção. H2s não renderiza, portanto, use **negrito** ou outras convenções para significar seções separadas.
1. Em seguida, preencha o texto do corpo usando o material de rascunho na seção Customer Insights da página Regra de Alquimia
    1. Listas com marcador estão ótimas
    1. Listas numeradas também
    1. **Negrito** *e itálico* são a-ok
    1. Os links sempre devem ser **"links para a Web"/links** **profundos** ou externos para elementos da interface do usuário, não links internos.
    1. As imagens não têm suporte oficial no momento, mas estão no roteiro.

E isso já é um pouco longo demais. A prática prática é de cerca de 400 caracteres ---------------------------------

Depois que o conteúdo estiver pronto, puxe-o para a ramificação ao vivo. Em seguida, vá para o portal do Parceiro [de Alquimia](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo url. 
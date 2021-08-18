---
title: Trocar seu site raiz clássico por um site moderno
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316128"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Trocar seu site raiz clássico por um site moderno

Se seu ambiente foi definido antes de abril de 2019, você pode alterar seu site raiz para um site moderno usando o Microsoft PowerShell:

- Se você tiver um site diferente que deseja usar como seu site raiz, poderá substituir [(trocar) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) por ele. 
    - Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site por outro site durante o arquivamento do site original. Disponível para Site de Equipe (não conectado a um grupo) e Site de Comunicação. 

- Recursos adicionais serão introduzidos em breve que permitirão que você continue usando o conteúdo no site, mas converta o site existente em um site de comunicação. 

**Importante:** esses recursos serão lançados gradualmente. Continue a verificar se o Centro de Mensagens está em busca de atualizações. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com a troca de sites

- O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo precisará ser recrucado para atualizar o índice de pesquisa. Não há nenhuma etapa manual necessária - isso será feito automaticamente.
- Qualquer coisa dependente de links "estáticos" (como a Sincronização de Arquivos e OneNote arquivos) precisará ser corrigido manualmente.
- Se o site de origem for um site de notícias organizacionais, atualize a URL. Obter uma lista de todos os sites de notícias organizacionais.
- Project Os sites de servidor podem precisar ser validados para garantir que eles ainda estão associados corretamente.

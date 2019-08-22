---
title: Trocar o site da raiz clássica por um site moderno
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501067"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Trocar o site da raiz clássica por um site moderno

Se seu ambiente tiver sido configurado antes de abril de 2019, você poderá alterar seu site raiz para um site moderno usando o Microsoft PowerShell:

- Se você tiver um site diferente que você deseja usar como seu site raiz, você pode substituir (trocar) o site raiz por ele. 
    - Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site com outro site enquanto arquiva o site original. Disponível para o site de equipe (não conectado a um grupo) e site de comunicação. 

- Recursos adicionais serão introduzidos em breve, permitindo que você continue usando o conteúdo do site, mas converta o site existente em um site de comunicação. 
>[!Important]
>Esses recursos serão implantados gradualmente. Continue a verificar o centro de mensagens do Office 365 para atualizações. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com o swap de sites

- O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo deverá ser rastreado para atualizar o índice de pesquisa. Não há nenhuma etapa manual necessária-isso será feito automaticamente.
- Qualquer coisa dependente de links "estáticos" (como sincronização de arquivos e arquivos do OneNote) precisará ser corrigida manualmente.
- Se o site de origem for um site de notícias organizacionais, atualize a URL.Obtenha uma lista de todos os sites de notícias organizacionais.
- Talvez seja necessário validar os sites do Project Server para garantir que eles ainda estejam associados corretamente.






---
title: Site moderno como o site raiz
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054690"
---
# <a name="modern-site-as-root-site"></a>Site moderno como site raiz

Começamos a implementar um novo recurso que permitirá [trocar seu site de raiz de site clássico por um site moderno](https://docs.microsoft.com/sharepoint/modern-root-site). Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site com outro site enquanto arquiva o site original. Disponível para o site de equipe (não conectado a um grupo) e site de comunicação.

>[!Important]
> Não exclua o site da raiz clássica para criar um site de comunicação moderno. Isso não é suportado pela Microsoft. A exclusão do site raiz tornará todos os sites do SharePoint em sua organização inacessíveis a todos os usuários, até que você restaure o site ou crie um novo site na mesma URL. Vamos comunicar esse recurso por meio do centro de mensagens. Você deve esperar que o recurso seja ativado em seu locatário em breve.

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com o swap de sites
- O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo deverá ser rastreado para atualizar o índice de pesquisa. Não é necessária nenhuma etapa manual aqui, isso será feito automaticamente.
- Qualquer coisa dependente de links "estáticos" (como sincronização de arquivos e arquivos do OneNote) precisará ser corrigida manualmente.
- Talvez seja necessário validar os sites do Project Server para garantir que eles ainda estejam associados corretamente. 

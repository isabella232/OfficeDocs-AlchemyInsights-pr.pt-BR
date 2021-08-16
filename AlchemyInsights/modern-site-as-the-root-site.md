---
title: Site moderno como o site raiz
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000374"
---
# <a name="modern-site-as-root-site"></a>Site moderno como site raiz

Começamos a lançar um novo recurso que permitirá que você troque seu site raiz de [site clássico por um site moderno.](https://docs.microsoft.com/sharepoint/modern-root-site) Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site por outro site durante o arquivamento do site original. Disponível para Site de Equipe (não conectado a um grupo) e Site de Comunicação.

>[!Important]
> Não exclua seu site raiz clássico para criar um Site de Comunicação moderno. Isso não é suportado pela Microsoft. Excluir o site raiz fará com que todos os sites SharePoint sua organização inacessíveis para todos os usuários, até que você restaure o site ou crie um novo site na mesma URL. Vamos comunicar esse recurso por meio do centro de mensagens. Você deve esperar que o recurso seja ligado em seu locatário em breve.

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com a troca de sites
- O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo precisará ser recrucado para atualizar o índice de pesquisa. Não há nenhuma etapa manual necessária aqui, isso será feito automaticamente.
- Qualquer coisa dependente de links "estáticos" (como a Sincronização de Arquivos e OneNote arquivos) precisará ser corrigido manualmente.
- Project Os sites de servidor podem precisar ser validados para garantir que eles ainda estão associados corretamente. 

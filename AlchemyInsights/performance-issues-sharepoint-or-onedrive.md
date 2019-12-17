---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068377"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários

O SharePoint ou o OneDrive podem ser lentos, inacessíveis ou indisponíveis, ou podem exibir serviços indisponíveis ou 503 erros, por vários motivos:
  
- Se seu site do SharePoint ou do OneDrive estiver lento ou atrasado para vários usuários, pode haver um problema de serviço temporário onde os usuários experimentam atrasos intermitentes ou erros de navegação ao acessar sites do SharePoint ou conteúdo do OneDrive. Verifique o [painel de integridade do serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização é afetada.
  
- Os usuários podem receber um erro de *servidor 503 está ocupado* ao tentar navegar até sites do SharePoint ou do onedrive. Esse erro pode ser causado pela limitação no serviço do SharePoint. SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online. O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos. Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Se você experimentar um desempenho lento com um **site ou uma** página do SharePoint moderno ou **moderna** , use a ferramenta de [diagnóstico de página](https://aka.ms/perftool) para analisar as páginas.
  
- Se você ainda tiver um desempenho mais lento, revise os recursos na parte inferior deste artigo: [introdução ao ajuste de desempenho para o SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  
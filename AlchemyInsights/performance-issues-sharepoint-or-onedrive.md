---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771889"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários

O SharePoint ou o OneDrive podem ser lentos, inacessíveis ou indisponíveis, ou podem exibir serviços indisponíveis ou 503 erros, por vários motivos:
  
- Se seu site do SharePoint ou do OneDrive estiver lento ou atrasado para vários usuários, pode haver um problema de serviço temporário onde os usuários experimentam atrasos intermitentes ou erros de navegação ao acessar sites do SharePoint ou conteúdo do OneDrive. Marque o [Painel de integridade do serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização é afetada.
  
- Os usuários podem receber um erro de *servidor 503 está ocupado* ao tentar navegar até sites do SharePoint ou do onedrive. Esse erro pode ser causado pela limitação no serviço do SharePoint. SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online. A limitação limita o número de ações do usuário ou de chamadas simultâneas (por script ou código) a fim de impedir o uso excessivo de recursos. Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Se você experimentar um desempenho lento com um **site ou uma** página do SharePoint moderno ou **moderna** , use a ferramenta de [diagnóstico de página](https://aka.ms/perftool) para analisar as páginas.
  
- Se você ainda tiver um desempenho mais lento, revise os recursos na parte inferior deste artigo: [introdução ao ajuste de desempenho para o SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  
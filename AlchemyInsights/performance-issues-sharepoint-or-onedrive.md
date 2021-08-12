---
title: Problemas de desempenho SharePoint ou OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911830"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários

SharePoint ou OneDrive podem ser lentos, inacessíveis ou indisponíveis ou podem exibir erros de serviço indisponíveis ou 503, por vários motivos:
  
- Se o site SharePoint ou OneDrive estiver lento ou atrasado para vários usuários, pode haver um problema de serviço temporário em que os usuários experimentam atrasos intermitentes ou erros de navegação ao acessar sites SharePoint ou OneDrive conteúdo. Marque o [Painel de integridade do serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização é afetada.
  
- Os usuários podem receber um erro de ocupado do *servidor 503* ao tentar navegar para SharePoint ou OneDrive sites. Esse erro pode ser causado pela 3ª vez no serviço de SharePoint. SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online. A limitação limita o número de ações do usuário ou de chamadas simultâneas (por script ou código) a fim de impedir o uso excessivo de recursos. Para obter mais informações sobre a aceleração, consulte Evite [ser barrado](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)ou bloqueado no SharePoint Online .

- Se você tiver um desempenho lento com **SharePoint** **um** site ou página clássico ou moderno, utilize a ferramenta [Diagnóstico](https://aka.ms/perftool) de Página para analisar as páginas.
  
- Se você ainda tiver um desempenho lento geral, revise os recursos na parte inferior deste artigo: Introdução ao ajuste de desempenho para SharePoint [Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  
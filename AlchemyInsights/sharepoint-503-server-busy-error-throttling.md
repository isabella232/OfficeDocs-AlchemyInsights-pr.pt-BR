---
title: Limitação do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742197"
---
# <a name="sharepoint-online-throttling"></a>Limitação do SharePoint Online

**Importante**: Durante esses tempos sem precedentes, estamos tomando medidas para garantir que os serviços do SharePoint Online e OneDrive permaneçam altamente disponíveis - Visite [Ajustes de recursos temporários do SharePoint Online](https://aka.ms/ODSPAdjustments) para obter mais informações.

**erro de servidor 503 está ocupado**

Os usuários podem receber um erro de servidor 503 está ocupado ao tentar navegar até sites do SharePoint ou do OneDrive. 

Esse erro pode ser causado pela limitação no serviço do SharePoint. SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online. O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos. 

Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Se acreditar que esse erro não está relacionado à limitação, você poderá verificar se há manutenção ativa ocorrendo no locatário, navegando até o [centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).

 Por fim, verifique se você está visitando a página [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar se há avisos/incidentes que possam ocorrer.


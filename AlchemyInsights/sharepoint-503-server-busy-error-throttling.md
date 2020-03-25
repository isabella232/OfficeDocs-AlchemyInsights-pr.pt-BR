---
title: Limitação do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931214"
---
# <a name="sharepoint-online-throttling"></a>Limitação do SharePoint Online

**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano. Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup. Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.

Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana. Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período. No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.

**erro de servidor 503 está ocupado**

Os usuários podem receber um erro de servidor 503 está ocupado ao tentar navegar até sites do SharePoint ou do OneDrive. 

Esse erro pode ser causado pela limitação no serviço do SharePoint. SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online. O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos. 

Para obter mais informações sobre limitação, confira o artigo sobre [como ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Se acreditar que esse erro não está relacionado à limitação, você poderá verificar se há manutenção ativa ocorrendo no locatário, navegando até o [centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).

 Por fim, verifique se você está visitando a página [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar se há avisos/incidentes que possam ocorrer.


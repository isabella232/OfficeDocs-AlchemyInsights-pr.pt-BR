---
title: Limitação do SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931430"
---
# <a name="sharepoint-online-throttling"></a>Limitação do SharePoint Online

**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano. Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup. Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.

Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana. Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período. No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.

**Limitação do SharePoint Online**

SharePoint Online usa a limitação para manter o melhor desempenho e confiabilidade do serviço SharePoint Online. O número de ações do usuário ou simultâneas redução dos limites chamadas (por script ou código) para impedir o uso excessivo de recursos. Para obter mais informações, visite os links abaixo.

- [Evite ficar limitado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Migração de dados e limitação de SPO](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [Velocidade de migração do SharePoint Online e do OneDrive](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [Controlar a limitação do SharePoint Online usando retirada exponencial](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [Planejamento de capacidade e teste de carregamento do SharePoint Online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)


---
title: Diretrizes de desempenho de migração geral
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932467"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="64095-102">Diretrizes de desempenho de migração geral</span><span class="sxs-lookup"><span data-stu-id="64095-102">General migration performance guidance</span></span>

<span data-ttu-id="64095-103">**Importante**: muitos clientes do SharePoint Online e do OneDrive executam, em segundo plano, aplicativos que usam o serviço e que são essenciais para os negócios.</span><span class="sxs-lookup"><span data-stu-id="64095-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="64095-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="64095-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="64095-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="64095-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="64095-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="64095-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="64095-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="64095-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="64095-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="64095-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="64095-109">**Diretrizes de desempenho da migração**</span><span class="sxs-lookup"><span data-stu-id="64095-109">**Migration performance guidance**</span></span>

<span data-ttu-id="64095-p103">O desempenho da migração pode será afetado pela infraestrutura de rede, tamanho do arquivo, período de migração e limitação. Noções básicas sobre esses ajudará a planejar e maximizar a eficácia da sua migração.</span><span class="sxs-lookup"><span data-stu-id="64095-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="64095-112">Diretrizes de desempenho de migração geral</span><span class="sxs-lookup"><span data-stu-id="64095-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

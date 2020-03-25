---
title: Migrar opções para o SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932718"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="45892-102">Migrar opções para o SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="45892-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="45892-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="45892-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="45892-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="45892-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="45892-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="45892-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="45892-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="45892-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="45892-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="45892-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="45892-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="45892-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="45892-109">**Opções de migração**</span><span class="sxs-lookup"><span data-stu-id="45892-109">**Migration options**</span></span>

<span data-ttu-id="45892-110">Há diferentes opções disponíveis para migrar o conteúdo para o SharePoint Online, dependendo do tamanho e da quantidade de arquivos que você precisa mover, confira uma lista de opções [localizadas aqui](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="45892-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="45892-111">Para obter mais informações sobre a migração de conteúdo, visite os links abaixo.</span><span class="sxs-lookup"><span data-stu-id="45892-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="45892-112">Ferramenta de migração do SharePoint</span><span class="sxs-lookup"><span data-stu-id="45892-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="45892-113">Introdução ao Gerenciador de Migração</span><span class="sxs-lookup"><span data-stu-id="45892-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="45892-114">Velocidade de migração do SharePoint Online e do ODB</span><span class="sxs-lookup"><span data-stu-id="45892-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="45892-115">Evite ficar limitado ou bloqueado no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="45892-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="45892-116">Ferramenta de avaliação de migração do SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="45892-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="45892-117">**Observação**: no momento, a ferramenta de migração do SharePoint oferece suporte a migrações do SharePoint 2010 e 2013.</span><span class="sxs-lookup"><span data-stu-id="45892-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="45892-118">Não há suporte para a versão 2016 ou 2019 no momento.</span><span class="sxs-lookup"><span data-stu-id="45892-118">Version 2016 or 2019 are not supported at this time.</span></span>

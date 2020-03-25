---
title: Solucionando problemas e erros da ferramenta de migração do SharePoint
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931106"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="b2811-102">Solucionando problemas e erros da ferramenta de migração do SharePoint</span><span class="sxs-lookup"><span data-stu-id="b2811-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="b2811-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="b2811-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b2811-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="b2811-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b2811-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="b2811-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b2811-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="b2811-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b2811-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="b2811-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b2811-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="b2811-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b2811-109">**Problemas e erros comuns**</span><span class="sxs-lookup"><span data-stu-id="b2811-109">**Common issues and errors**</span></span>

<span data-ttu-id="b2811-110">Você pode encontrar alguns problemas e erros comuns ao usar a ferramenta de migração do SharePoint (SPMT).</span><span class="sxs-lookup"><span data-stu-id="b2811-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="b2811-111">Consulte os links abaixo para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="b2811-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="b2811-112">Solucionar problemas e erros comuns da SPMT</span><span class="sxs-lookup"><span data-stu-id="b2811-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="b2811-113">Solucionando problemas de instalação do SPMT</span><span class="sxs-lookup"><span data-stu-id="b2811-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)
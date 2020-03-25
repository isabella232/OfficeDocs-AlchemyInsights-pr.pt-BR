---
title: Limitação de migração do SharePoint com erros 503
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931646"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="0542e-102">Limitação de migração do SharePoint com erros 503</span><span class="sxs-lookup"><span data-stu-id="0542e-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="0542e-103">**Importante**: muitos clientes do SharePoint Online e do onedrive executam aplicativos críticos para os negócios em relação ao serviço executado em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="0542e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0542e-104">Isso inclui a migração de conteúdo, a DLP (prevenção de perda de dados) e as soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="0542e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0542e-105">Durante esses tempos sem precedentes, estamos tomando as medidas necessárias para garantir que os serviços do SharePoint Online e do OneDrive permaneçam altamente disponíveis e confiáveis aos usuários que dependem mais do que nunca do serviço em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="0542e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0542e-106">Em suporte a esse objetivo, implementamos limites mais apertados nas aplicações de segundo plano (soluções de migração, DLP e backup) durante as horas úteis da semana.</span><span class="sxs-lookup"><span data-stu-id="0542e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0542e-107">Você deve esperar que esses aplicativos atinjam uma taxa de transferência mais limitada durante esse período.</span><span class="sxs-lookup"><span data-stu-id="0542e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0542e-108">No entanto, durante a noite e nos fins de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicativos em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="0542e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0542e-109">**503 erros ao migrar para o SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="0542e-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="0542e-110">Parece que você está migrando para o SharePoint Online e recebendo erros 503.</span><span class="sxs-lookup"><span data-stu-id="0542e-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="0542e-111">Siga as etapas abaixo para que possamos ajudá-lo assim que possível.</span><span class="sxs-lookup"><span data-stu-id="0542e-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="0542e-112">Clique em **entrar em contato com o suporte**e em **nova solicitação de serviço**.</span><span class="sxs-lookup"><span data-stu-id="0542e-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="0542e-113">Para o título e a descrição, digite **limitação de migração do SharePoint com 503**.</span><span class="sxs-lookup"><span data-stu-id="0542e-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="0542e-114">Depois que o tíquete for enviado, atualize-o com as seguintes informações:</span><span class="sxs-lookup"><span data-stu-id="0542e-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="0542e-115">Quanto à esquerda da migração (por exemplo, Quantos TBs?).</span><span class="sxs-lookup"><span data-stu-id="0542e-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="0542e-116">Data de início e de término da migração.</span><span class="sxs-lookup"><span data-stu-id="0542e-116">Migration start and end date.</span></span>
    - <span data-ttu-id="0542e-117">Descrever de onde você está migrando seu conteúdo, como o SharePoint Server, Box, GDrive, compartilhamentos de arquivos, etc..</span><span class="sxs-lookup"><span data-stu-id="0542e-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="0542e-118">Estimar o número de erros de limitação (por exemplo, o acelerador x por hora?) e quando a limitação aconteceu.</span><span class="sxs-lookup"><span data-stu-id="0542e-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="0542e-119">Qual ferramenta de migração você está usando (por exemplo, SPMT ou ShareGate).</span><span class="sxs-lookup"><span data-stu-id="0542e-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>



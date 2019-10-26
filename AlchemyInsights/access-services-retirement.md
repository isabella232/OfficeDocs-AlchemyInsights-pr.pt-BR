---
title: Aposentadoria de serviços do Access
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747772"
---
# <a name="access-services-retirement"></a><span data-ttu-id="305b0-102">Aposentadoria de serviços do Access</span><span class="sxs-lookup"><span data-stu-id="305b0-102">Access services retirement</span></span>

<span data-ttu-id="305b0-103">Como anunciamos originalmente no MC97576, em março de 2017, e continuamos a se comunicar nos serviços de acesso do ano passado estão sendo retirados do Office 365.</span><span class="sxs-lookup"><span data-stu-id="305b0-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="305b0-104">A próxima fase desse processo será a remoção dos bancos de dados do Access Web que usam as listas do SharePoint como armazenamento de dados subjacente.</span><span class="sxs-lookup"><span data-stu-id="305b0-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="305b0-105">**Como isso me afeta?**</span><span class="sxs-lookup"><span data-stu-id="305b0-105">**How does this affect me?**</span></span>

<span data-ttu-id="305b0-106">A partir de junho de 2019, implantaremos a criação de novos bancos de dados do Access no SharePoint Online e encerrará o serviço e todos os aplicativos restantes em abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="305b0-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="305b0-107">**O que eu preciso fazer para se preparar para essa alteração?**</span><span class="sxs-lookup"><span data-stu-id="305b0-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="305b0-108">Recomendamos que você crie um plano de transição para os bancos de dados de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="305b0-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="305b0-109">Os administradores podem usar o [Verificador de aplicativos do Access do SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário dos aplicativos do Access que os sites estão usando.</span><span class="sxs-lookup"><span data-stu-id="305b0-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="305b0-110">Há várias maneiras de migrar os dados dos bancos de dados da Web do Access:</span><span class="sxs-lookup"><span data-stu-id="305b0-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="305b0-111">Importando para um banco de dados de acesso local (. ACCDB) ou para um arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="305b0-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="305b0-112">Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócios sem código para dispositivos da Web e móveis.</span><span class="sxs-lookup"><span data-stu-id="305b0-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>
---
title: Aposentadoria de serviços do Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973896"
---
# <a name="access-services-retirement"></a><span data-ttu-id="f8ee3-102">Aposentadoria de serviços do Access</span><span class="sxs-lookup"><span data-stu-id="f8ee3-102">Access services retirement</span></span>

<span data-ttu-id="f8ee3-103">Como anunciamos originalmente no MC97576, em março de 2017, e continuamos a se comunicar nos serviços de acesso do ano passado estão sendo retirados do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f8ee3-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="f8ee3-104">A próxima fase desse processo será a remoção dos bancos de dados do Access Web que usam as listas do SharePoint como armazenamento de dados subjacente.</span><span class="sxs-lookup"><span data-stu-id="f8ee3-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="f8ee3-105">Como isso me afeta?</span><span class="sxs-lookup"><span data-stu-id="f8ee3-105">How does this affect me?</span></span>

<span data-ttu-id="f8ee3-106">A partir de junho de 2019, implantaremos a criação de novos bancos de dados do Access no SharePoint Online e encerrará o serviço e todos os aplicativos restantes em abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="f8ee3-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="f8ee3-107">O que eu preciso fazer para se preparar para essa alteração?</span><span class="sxs-lookup"><span data-stu-id="f8ee3-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="f8ee3-108">Recomendamos que você crie um plano de transição para os bancos de dados de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="f8ee3-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="f8ee3-109">Os administradores podem usar o verificador de [aplicativos do Access do SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) para obter um inventário dos aplicativos do Access que os sites estão usando.</span><span class="sxs-lookup"><span data-stu-id="f8ee3-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="f8ee3-110">Há várias maneiras de migrar os dados dos bancos de dados da Web do Access:</span><span class="sxs-lookup"><span data-stu-id="f8ee3-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="f8ee3-111">Importando para um banco de dados de acesso local (. ACCDB) ou para um arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="f8ee3-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="f8ee3-112">Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócios sem código para dispositivos da Web e móveis.</span><span class="sxs-lookup"><span data-stu-id="f8ee3-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>
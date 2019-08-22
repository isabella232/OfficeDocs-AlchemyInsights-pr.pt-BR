---
title: Aposentadoria de serviços do Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495739"
---
# <a name="access-services-retirement"></a><span data-ttu-id="f41b6-102">Aposentadoria de serviços do Access</span><span class="sxs-lookup"><span data-stu-id="f41b6-102">Access services retirement</span></span>

<span data-ttu-id="f41b6-103">Como anunciamos originalmente no MC97576, em março de 2017, e continuamos a se comunicar nos serviços de acesso do ano passado estão sendo retirados do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f41b6-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="f41b6-104">A próxima fase desse processo será a remoção dos bancos de dados do Access Web que usam as listas do SharePoint como armazenamento de dados subjacente.</span><span class="sxs-lookup"><span data-stu-id="f41b6-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="f41b6-105">**Como isso me afeta?**</span><span class="sxs-lookup"><span data-stu-id="f41b6-105">**How does this affect me?**</span></span>

<span data-ttu-id="f41b6-106">A partir de junho de 2019, implantaremos a criação de novos bancos de dados do Access no SharePoint Online e encerrará o serviço e todos os aplicativos restantes em abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="f41b6-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="f41b6-107">**O que eu preciso fazer para se preparar para essa alteração?**</span><span class="sxs-lookup"><span data-stu-id="f41b6-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="f41b6-108">Recomendamos que você crie um plano de transição para os bancos de dados de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="f41b6-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="f41b6-109">Os administradores podem usar o verificador de [aplicativos do Access do SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário dos aplicativos do Access que os sites estão usando.</span><span class="sxs-lookup"><span data-stu-id="f41b6-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="f41b6-110">Há várias maneiras de migrar os dados dos bancos de dados da Web do Access:</span><span class="sxs-lookup"><span data-stu-id="f41b6-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="f41b6-111">Importando para um banco de dados de acesso local (. ACCDB) ou para um arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="f41b6-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="f41b6-112">Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócios sem código para dispositivos da Web e móveis.</span><span class="sxs-lookup"><span data-stu-id="f41b6-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>
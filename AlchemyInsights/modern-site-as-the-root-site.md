---
title: Site moderno como o site raiz
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057667"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="b1709-102">Site moderno como site raiz</span><span class="sxs-lookup"><span data-stu-id="b1709-102">Modern site as root site</span></span>

<span data-ttu-id="b1709-103">Os clientes de [lançamento de destino](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) agora podem habilitar a experiência de site de comunicação moderna no site raiz clássico do locatário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b1709-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="b1709-104">Esse recurso pode ser ativado executando um cmdlet simples do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b1709-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="b1709-105">Na execução bem-sucedida dos comandos do PowerShell, o site raiz terá uma nova home page do site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="b1709-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="b1709-106">Os detalhes sobre o cmdlet do PowerShell e os requisitos de recursos estão disponíveis no artigo [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="b1709-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="b1709-107">Vamos reverter isso, por padrão, para clientes de lançamento direcionado no início de maio de 2019, e a implantação estará disponível em todo o mundo no final de 2019 de junho.</span><span class="sxs-lookup"><span data-stu-id="b1709-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="b1709-108">Continue referindo-se ao [centro de mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) para outros novos recursos com o moderno.</span><span class="sxs-lookup"><span data-stu-id="b1709-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="b1709-109">**Importante**: não exclua o site da raiz clássica para criar um site de comunicação moderno.</span><span class="sxs-lookup"><span data-stu-id="b1709-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="b1709-110">Isso não é suportado pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1709-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="b1709-111">A exclusão do site raiz tornará todos os sites do SharePoint em sua organização inacessíveis a todos os usuários, até que você restaure o site ou crie um novo site na mesma URL.</span><span class="sxs-lookup"><span data-stu-id="b1709-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 
---
title: Restringir o modo clássico do SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761747"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="86f80-102">Restringir o modo clássico do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="86f80-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="86f80-103">Algumas organizações ainda exigem a experiência de modo clássico.</span><span class="sxs-lookup"><span data-stu-id="86f80-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="86f80-104">Embora não haja planos de remover o modo clássico em um nível granular, não é mais possível restringir uma organização inteira (locatário) a um modo clássico para listas e bibliotecas.</span><span class="sxs-lookup"><span data-stu-id="86f80-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="86f80-105">O administrador terá as seguintes opções para gerenciar listas e bibliotecas individuais no modo clássico usando opções de recusa granular que fornecemos nos seguintes níveis:</span><span class="sxs-lookup"><span data-stu-id="86f80-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="86f80-106">conjunto de sites</span><span class="sxs-lookup"><span data-stu-id="86f80-106">site collection</span></span>
- <span data-ttu-id="86f80-107">no</span><span class="sxs-lookup"><span data-stu-id="86f80-107">site</span></span>
- <span data-ttu-id="86f80-108">list</span><span class="sxs-lookup"><span data-stu-id="86f80-108">list</span></span>
- <span data-ttu-id="86f80-109">Libra</span><span class="sxs-lookup"><span data-stu-id="86f80-109">library</span></span>

<span data-ttu-id="86f80-110">Além disso, as listas que usam determinados recursos e personalizações que não são suportadas pela moderna ainda serão automaticamente alternadas para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="86f80-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="86f80-111">A partir de 1º de abril de 2019, o processo para desativar o consentimento de nível de locatário de listas e bibliotecas modernas começará e continuará em 31 de maio de 2019.</span><span class="sxs-lookup"><span data-stu-id="86f80-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="86f80-112">As listas e bibliotecas que estão no modo clássico como resultado da recusa do locatário serão automaticamente deslocadas para o moderno.</span><span class="sxs-lookup"><span data-stu-id="86f80-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="86f80-113">Se você precisar do modo clássico, Confira mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instruções do PowerShell do PNP [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descrevem as opções e ferramentas que você pode usar atualmente para usar a experiência de modo clássico.</span><span class="sxs-lookup"><span data-stu-id="86f80-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>

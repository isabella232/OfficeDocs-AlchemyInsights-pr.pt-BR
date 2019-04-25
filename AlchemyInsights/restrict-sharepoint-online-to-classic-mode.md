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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32422163"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="9923d-102">Restringir o modo clássico do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9923d-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="9923d-103">Algumas organizações ainda exigem a experiência de modo clássico.</span><span class="sxs-lookup"><span data-stu-id="9923d-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="9923d-104">Embora não haja planos para remover o modo clássico em um nível granular, Iniciando em 1º de abril de 2019, não será mais possível restringir uma organização inteira (locatário) a um modo clássico para listas e bibliotecas.</span><span class="sxs-lookup"><span data-stu-id="9923d-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="9923d-105">O administrador terá as seguintes opções para gerenciar listas e bibliotecas individuais no modo clássico usando opções de recusa granular que fornecemos nos seguintes níveis:</span><span class="sxs-lookup"><span data-stu-id="9923d-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="9923d-106">conjunto de sites</span><span class="sxs-lookup"><span data-stu-id="9923d-106">site collection</span></span>
- <span data-ttu-id="9923d-107">site</span><span class="sxs-lookup"><span data-stu-id="9923d-107">site</span></span>
- <span data-ttu-id="9923d-108">list</span><span class="sxs-lookup"><span data-stu-id="9923d-108">list</span></span>
- <span data-ttu-id="9923d-109">Libra</span><span class="sxs-lookup"><span data-stu-id="9923d-109">library</span></span>

<span data-ttu-id="9923d-110">Além disso, as listas que usam determinados recursos e personalizações que não são suportadas pela moderna ainda serão automaticamente alternadas para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="9923d-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="9923d-111">Após 1º de abril, as listas e bibliotecas que estão no modo clássico como resultado de recusa do locatário serão automaticamente gerenciadas no nível do site e na lista.</span><span class="sxs-lookup"><span data-stu-id="9923d-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="9923d-112">Se você precisar do modo clássico, Confira mais informações aqui e instruções do PowerShell do PnP aqui que descrevem as opções e ferramentas que você pode usar atualmente para se preparar para a remoção da aceitação do nível do locatário em 1º de abril.</span><span class="sxs-lookup"><span data-stu-id="9923d-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>

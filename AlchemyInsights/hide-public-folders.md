---
title: Ocultar pastas públicas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294635"
---
# <a name="hide-public-folders"></a><span data-ttu-id="c859f-102">Ocultar pastas públicas</span><span class="sxs-lookup"><span data-stu-id="c859f-102">Hide public folders</span></span>

<span data-ttu-id="c859f-103">**Para ocultar toda a árvore de pastas públicas**:</span><span class="sxs-lookup"><span data-stu-id="c859f-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="c859f-104">Use as etapas [neste](https://aka.ms/ControlPF) artigo para ocultar a árvore de pasta pública inteira de usuários seletivos ou de todos.</span><span class="sxs-lookup"><span data-stu-id="c859f-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="c859f-105">**Para ocultar uma pasta pública específica**:</span><span class="sxs-lookup"><span data-stu-id="c859f-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="c859f-106">Adicionar permissões para usuários que precisam acessar a pasta pública</span><span class="sxs-lookup"><span data-stu-id="c859f-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="c859f-107">Remova o **Padrão** do usuário da **lista de permissões**:</span><span class="sxs-lookup"><span data-stu-id="c859f-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`

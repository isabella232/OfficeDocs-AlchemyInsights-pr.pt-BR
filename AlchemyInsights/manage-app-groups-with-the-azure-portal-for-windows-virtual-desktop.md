---
title: Gerenciar grupos de aplicativos usando o portal do Azure para a área de trabalho virtual do Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715657"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="02aaa-102">Gerenciar grupos de aplicativos usando o portal do Azure para a área de trabalho virtual do Windows</span><span class="sxs-lookup"><span data-stu-id="02aaa-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="02aaa-103">O grupo de aplicativos padrão criado para um novo pool de hosts de área de trabalho virtual do Windows também publica a área de trabalho completa.</span><span class="sxs-lookup"><span data-stu-id="02aaa-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="02aaa-104">Além disso, o uso do portal do Azure permite que você crie um ou mais grupos de aplicativos RemoteApp para o pool de hosts.</span><span class="sxs-lookup"><span data-stu-id="02aaa-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="02aaa-105">O processo de implantação fará o seguinte:</span><span class="sxs-lookup"><span data-stu-id="02aaa-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="02aaa-106">Crie o grupo de aplicativos do RemoteApp.</span><span class="sxs-lookup"><span data-stu-id="02aaa-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="02aaa-107">Adicione seus aplicativos selecionados ao grupo de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="02aaa-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="02aaa-108">Publique usuários individuais ou grupos de usuários no grupo de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="02aaa-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="02aaa-109">Registre o grupo de aplicativos, se você optar por fazer isso.</span><span class="sxs-lookup"><span data-stu-id="02aaa-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="02aaa-110">Crie um link para um modelo do Azure Resource Manager de acordo com sua configuração, que você pode baixar e salvar.</span><span class="sxs-lookup"><span data-stu-id="02aaa-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="02aaa-111">Para criar um grupo RemoteApp para a área de trabalho virtual do Windows, siga as instruções em [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span><span class="sxs-lookup"><span data-stu-id="02aaa-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>

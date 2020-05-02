---
title: Canal privado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005426"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="0d197-102">Canais privados no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0d197-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="0d197-103">Os canais privados são um novo recurso no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0d197-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="0d197-104">Observe que os canais privados não podem ser convertidos de canais padrão ou vice-versa.</span><span class="sxs-lookup"><span data-stu-id="0d197-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="0d197-105">Para obter detalhes sobre canais privados, como informações sobre [criação de canal privado e](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [sites do SharePoint de canal privado](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), consulte [canais privados no Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="0d197-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="0d197-106">**Observação:** Como a configuração para retenção de mensagens de canal privado ainda não é suportada, os locatários com políticas de retenção habilitadas não terão canais privados habilitados por padrão.</span><span class="sxs-lookup"><span data-stu-id="0d197-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="0d197-107">Os canais privados podem ser habilitados no centro de administração do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0d197-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="0d197-108">Além disso, observe que, enquanto a retenção de mensagens de canal privado não é suportada, a retenção de arquivos compartilhados em canais privados é suportada.</span><span class="sxs-lookup"><span data-stu-id="0d197-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="0d197-109">**Precisa de um novo proprietário de equipe?**</span><span class="sxs-lookup"><span data-stu-id="0d197-109">**Need a new team owner?**</span></span>

<span data-ttu-id="0d197-110">Se o proprietário do seu canal privado sair, você poderá adicionar um novo proprietário da equipe via Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0d197-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="0d197-111">Vá [aqui](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) para instalar o Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0d197-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="0d197-112">Aqui está o cmdlet que você precisará:</span><span class="sxs-lookup"><span data-stu-id="0d197-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="0d197-113">Para obter mais informações sobre o Teams PowerShell, consulte [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="0d197-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>

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
# <a name="private-channels-in-microsoft-teams"></a>Canais privados no Microsoft Teams

Os canais privados são um novo recurso no Microsoft Teams. Observe que os canais privados não podem ser convertidos de canais padrão ou vice-versa.

Para obter detalhes sobre canais privados, como informações sobre [criação de canal privado e](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [sites do SharePoint de canal privado](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), consulte [canais privados no Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Observação:** Como a configuração para retenção de mensagens de canal privado ainda não é suportada, os locatários com políticas de retenção habilitadas não terão canais privados habilitados por padrão. Os canais privados podem ser habilitados no centro de administração do Microsoft Teams. Além disso, observe que, enquanto a retenção de mensagens de canal privado não é suportada, a retenção de arquivos compartilhados em canais privados é suportada.

**Precisa de um novo proprietário de equipe?**

Se o proprietário do seu canal privado sair, você poderá adicionar um novo proprietário da equipe via Teams PowerShell.


- Vá [aqui](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) para instalar o Teams PowerShell.

Aqui está o cmdlet que você precisará:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Para obter mais informações sobre o Teams PowerShell, consulte [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).

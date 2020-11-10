---
title: Usando o Giphys em conversas do teams
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947474"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="3e445-102">Usando o Giphys em conversas do teams</span><span class="sxs-lookup"><span data-stu-id="3e445-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="3e445-103">O acesso Giphys no Microsoft Teams está habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="3e445-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="3e445-104">Como administrador, você pode controlar se o Giphys está disponível para os usuários [Configurando uma política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) e garantindo que o **uso do Giphys em conversas** esteja **ativado**.</span><span class="sxs-lookup"><span data-stu-id="3e445-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="3e445-105">Se GIFs não estiverem funcionando conforme o esperado nas conversas de equipes, verifique:</span><span class="sxs-lookup"><span data-stu-id="3e445-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="3e445-106">A [política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) precisa permitir o Giphys.</span><span class="sxs-lookup"><span data-stu-id="3e445-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="3e445-107">Para verificar usando os cmdlets do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3e445-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="3e445-108">Verifique se você pode [gerenciar o Microsoft Teams com o PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="3e445-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="3e445-109">Execute o comando do PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verifique se **AllowGiphy** está definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="3e445-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="3e445-110">Se **AllowGiphy** estiver definido como **false** , execute o seguinte comando [set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3e445-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="3e445-111">[Experiências conectadas opcionais](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) precisam ser habilitadas para permitir o acesso à URL do Giphy.</span><span class="sxs-lookup"><span data-stu-id="3e445-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="3e445-112">Se você tiver várias políticas de mensagens do Microsoft Teams configuradas para seu locatário, é possível determinar a identidade da política atribuída ao usuário afetado com o comando [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | do PowerShell. <user@domain.com> Selecione TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="3e445-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>

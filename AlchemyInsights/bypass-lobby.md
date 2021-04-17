---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820022"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="eb886-102">Controlar configurações de lobby e nível de participação no Teams</span><span class="sxs-lookup"><span data-stu-id="eb886-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="eb886-103">Se você quiser permitir que todos, incluindo usuários dial-in, externos e anônimos, ignorem o **lobby,** use o PowerShell para realizar essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="eb886-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="eb886-104">Aqui está um exemplo de modificação da política de reunião global para sua organização.</span><span class="sxs-lookup"><span data-stu-id="eb886-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="eb886-105">Atualmente, esse cmdlet requer o uso do módulo Do PowerShell do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="eb886-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="eb886-106">Para configurar para usar esse cmdlet, confira [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="eb886-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="eb886-107">Depois de configurar uma política, você precisa aplicá-la aos usuários; ou, se você modificou a política Global, ela será automaticamente aplicada aos usuários.</span><span class="sxs-lookup"><span data-stu-id="eb886-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="eb886-108">Para qualquer alteração de política, você precisa aguardar pelo menos 4 horas até **24** horas para que as políticas entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="eb886-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="eb886-109">Não deixe de revisar a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.</span><span class="sxs-lookup"><span data-stu-id="eb886-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="eb886-110">Noções básicas sobre controles de política de lobby de reunião do Teams</span><span class="sxs-lookup"><span data-stu-id="eb886-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="eb886-111">Essas configurações controlam quais participantes da reunião aguardam no lobby antes de ser admitidos na reunião e o nível de participação que eles são permitidos em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="eb886-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="eb886-112">Você pode usar o PowerShell para atualizar as configurações de política de reunião que ainda não foram implementadas (rotuladas como "em breve") no centro de administração do Teams.</span><span class="sxs-lookup"><span data-stu-id="eb886-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="eb886-113">Confira abaixo um exemplo de cmdlet do PowerShell que permite que todos os usuários ignorem o lobby.</span><span class="sxs-lookup"><span data-stu-id="eb886-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="eb886-114">[Admitir automaticamente que](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) as pessoas são uma política por organizador que controla se as pessoas ingressarão em uma reunião diretamente ou aguardarão no lobby até que sejam admitidas por um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="eb886-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="eb886-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Permitir que pessoas anônimas iniciem uma reunião é uma política por organizador que controla se pessoas anônimas, incluindo usuários B2B e federados, podem ingressar na reunião do usuário sem um usuário autenticado da organização presente.</span><span class="sxs-lookup"><span data-stu-id="eb886-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="eb886-116">Permitir que os usuários de discagem ignorem o lobby **(** em breve ) é uma política por organizador que  controla se as pessoas que discam por telefone in unem a reunião diretamente ou aguardam no [lobby,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) independentemente da configuração Admitir automaticamente as pessoas.</span><span class="sxs-lookup"><span data-stu-id="eb886-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="eb886-117">Permitir que os organizadores substituam as configurações de [lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(** em breve ) é uma política  por organizador que controla se o organizador da reunião pode substituir as configurações de lobby definidas por um administrador em Automaticamente admitir pessoas e permitir que os usuários de discagem ignorem o **lobby** quando agendam uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="eb886-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="eb886-118">**Observação:** Leia [Gerenciar políticas de reunião no Teams para](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) uma visão geral completa das políticas de reunião do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eb886-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

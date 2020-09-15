---
title: Ignorar lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684938"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="cb22f-102">Controlar as configurações de lobby e o nível de participação no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cb22f-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="cb22f-103">Se quiser permitir que todos, incluindo usuários de discagem, externos e anônimos, **ignore o lobby**, use o PowerShell para realizar essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="cb22f-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="cb22f-104">Veja um exemplo de modificação da política de reunião global para sua organização.</span><span class="sxs-lookup"><span data-stu-id="cb22f-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="cb22f-105">Atualmente, este cmdlet requer o uso do módulo PowerShell do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="cb22f-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="cb22f-106">Para ser configurado para usar este cmdlet, confira o [Gerenciamento de políticas por meio do PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="cb22f-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="cb22f-107">Depois de configurar uma política, você precisa aplicá-la aos usuários; ou, se você modificou a política global, ela será automaticamente aplicada aos usuários.</span><span class="sxs-lookup"><span data-stu-id="cb22f-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="cb22f-108">Para qualquer alteração de política, você precisa aguardar pelo menos **4 horas até 24 horas** para que as políticas entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="cb22f-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="cb22f-109">Leia a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.</span><span class="sxs-lookup"><span data-stu-id="cb22f-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="cb22f-110">Noções básicas sobre controles de política de lobby de reunião de equipe</span><span class="sxs-lookup"><span data-stu-id="cb22f-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="cb22f-111">Essas configurações controlam quais participantes da reunião esperam no lobby antes de serem admitidos na reunião e o nível de participação que eles são permitidos em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="cb22f-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="cb22f-112">Você pode usar o PowerShell para atualizar as configurações de política de reunião que ainda não foram implementadas (rotuladas "em breve") no centro de administração do teams.</span><span class="sxs-lookup"><span data-stu-id="cb22f-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="cb22f-113">Veja a seguir um exemplo de cmdlet do PowerShell que permite que todos os usuários ignorem o lobby.</span><span class="sxs-lookup"><span data-stu-id="cb22f-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="cb22f-114">[Admitir pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas ingressam em uma reunião diretamente ou esperam no lobby até que sejam admitidas por um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="cb22f-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="cb22f-115">[Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo usuários B2B e federados, podem participar da reunião do usuário sem um usuário autenticado da organização em atendimento.</span><span class="sxs-lookup"><span data-stu-id="cb22f-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="cb22f-116">[Permitir que os usuários discados ignorem o lobby (em](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **breve**) é uma política por organizador que controla se as pessoas que discam por telefone ingressam na reunião diretamente ou esperam no lobby independentemente da configuração **admitir pessoas automaticamente** .</span><span class="sxs-lookup"><span data-stu-id="cb22f-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="cb22f-117">[Permitir que os organizadores substituam as configurações de lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (em**breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações de lobby de que um administrador definido **automaticamente admite pessoas** e **permitir que os usuários de discagem ignorem o lobby** quando agendarem uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="cb22f-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="cb22f-118">**Observação:** Leia [gerenciar políticas de reunião no Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das políticas de reunião do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cb22f-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

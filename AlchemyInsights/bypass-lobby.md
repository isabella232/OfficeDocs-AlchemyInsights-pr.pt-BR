---
title: Ignorar lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768428"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="15d59-102">Controlar configurações de lobby e nível de participação</span><span class="sxs-lookup"><span data-stu-id="15d59-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="15d59-103">Se quiser permitir que todos, incluindo usuários de discagem, externos e anônimos consigam o lobby no Microsoft Teams, você pode usar o PowerShell para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="15d59-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="15d59-104">Veja um exemplo de como modificar a política de reunião global para sua organização:</span><span class="sxs-lookup"><span data-stu-id="15d59-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="15d59-105">Atualmente, este cmdlet requer o uso do módulo PowerShell do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="15d59-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="15d59-106">Para fazer com que a instalação Use este cmdlet, confira [Gerenciamento de políticas por meio do PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="15d59-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="15d59-107">Você pode configurar uma nova política, que deverá ser aplicada aos usuários.</span><span class="sxs-lookup"><span data-stu-id="15d59-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="15d59-108">Se você modificar a política global, ela será automaticamente aplicada aos usuários.</span><span class="sxs-lookup"><span data-stu-id="15d59-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="15d59-109">Para qualquer alteração de política, você precisa aguardar pelo menos 4 horas e até 24 horas para que as políticas entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="15d59-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="15d59-110">Leia a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.</span><span class="sxs-lookup"><span data-stu-id="15d59-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="15d59-111">Noções básicas sobre controles de política de lobby de reunião de equipe</span><span class="sxs-lookup"><span data-stu-id="15d59-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="15d59-112">[Admitir pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas ingressam em uma reunião diretamente ou esperam no lobby até que sejam admitidas por um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="15d59-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="15d59-113">[Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo usuários B2B e federados, podem participar da reunião do usuário sem um usuário autenticado da organização em atendimento.</span><span class="sxs-lookup"><span data-stu-id="15d59-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="15d59-114">[Permitir que os usuários discados ignorem o lobby (em](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **breve**) é uma política por organizador que controla se as pessoas que discam por telefone ingressam na reunião diretamente ou esperam no lobby independentemente da configuração **admitir pessoas automaticamente** .</span><span class="sxs-lookup"><span data-stu-id="15d59-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="15d59-115">[Permitir que os organizadores substituam as configurações de lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (em**breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações de lobby de que um administrador definido em **admitir pessoas** e **permitir discagem os usuários ignoram o lobby** quando eles agendam uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="15d59-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="15d59-116">**Observação:** Leia [gerenciar políticas de reunião no Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das políticas de reunião do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="15d59-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

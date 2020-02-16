---
title: Configurações de política de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042832"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="c6667-102">Gerenciar políticas de reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c6667-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="c6667-103">**Observação: pode levar até 24 horas para que as alterações de política entrem em vigor para os usuários.**</span><span class="sxs-lookup"><span data-stu-id="c6667-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="c6667-104">Você pode não conseguir fazer alterações em políticas recentemente criadas imediatamente; Aguarde 4 horas e tente modificar novamente uma política recém-criada.</span><span class="sxs-lookup"><span data-stu-id="c6667-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="c6667-105">As políticas de reunião são usadas para controlar os recursos disponíveis para os participantes da reunião para reuniões agendadas por usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="c6667-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="c6667-106">Alguns recursos das políticas de reunião podem não ser implementados no centro de administração do teams ainda (eles estão "em breve" na documentação).</span><span class="sxs-lookup"><span data-stu-id="c6667-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="c6667-107">Nesse caso, ou se você estiver recebendo um erro como "não é possível atualizar a política agora, mas tentar novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar as políticas de reunião do teams.</span><span class="sxs-lookup"><span data-stu-id="c6667-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="c6667-108">Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="c6667-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="c6667-109">Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, confira [gerenciar políticas de reunião no Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="c6667-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="c6667-110">Para fazer alterações de política usando cmdlets do PowerShell, consulte [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="c6667-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="c6667-111">Você precisa usar o [módulo PowerShell do Skype for Business](https://www.microsoft.com/download/details.aspx?id=39366) para as políticas de reunião do teams.</span><span class="sxs-lookup"><span data-stu-id="c6667-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="c6667-112">Consulte a [documentação dos cmdlets do \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="c6667-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>


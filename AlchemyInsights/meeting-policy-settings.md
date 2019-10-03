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
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376508"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ab4ec-102">Gerenciar políticas de reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ab4ec-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ab4ec-103">As políticas de reunião são usadas para controlar os recursos disponíveis para os participantes da reunião para reuniões agendadas por usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ab4ec-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ab4ec-104">Alguns recursos das políticas de reunião podem não ser implementados no centro de administração do teams ainda (eles estão "em breve" na documentação).</span><span class="sxs-lookup"><span data-stu-id="ab4ec-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ab4ec-105">Nesse caso, ou se você estiver recebendo um erro como "não é possível atualizar a política agora, mas tentar novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar as políticas de reunião do teams.</span><span class="sxs-lookup"><span data-stu-id="ab4ec-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ab4ec-106">Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="ab4ec-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ab4ec-107">Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, confira [gerenciar políticas de reunião no Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ab4ec-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ab4ec-108">Para fazer alterações de política usando cmdlets do PowerShell, consulte [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ab4ec-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ab4ec-109">Você precisa usar o [módulo PowerShell do Skype for Business](https://www.microsoft.com/download/details.aspx?id=39366) para as políticas de reunião do teams.</span><span class="sxs-lookup"><span data-stu-id="ab4ec-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ab4ec-110">Consulte a [documentação dos cmdlets do \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ab4ec-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="ab4ec-111">**Observação:** Pode levar até 24 horas para que as alterações de política entrem em vigor para os usuários.</span><span class="sxs-lookup"><span data-stu-id="ab4ec-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="ab4ec-112">Você pode não conseguir fazer alterações em políticas recentemente criadas imediatamente; Aguarde 4 horas e tente modificar novamente uma política recém-criada.</span><span class="sxs-lookup"><span data-stu-id="ab4ec-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="ab4ec-113">Se você ainda tiver problemas, experimente o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ab4ec-113">If you're still having problems, try PowerShell.</span></span>  
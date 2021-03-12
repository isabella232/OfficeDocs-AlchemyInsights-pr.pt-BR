---
title: Configurações de política de reunião
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704594"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="24ed8-102">Gerenciar políticas de reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="24ed8-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="24ed8-103">**Observação: pode levar até 24 horas para que as alterações de política entre em vigor para os usuários.**</span><span class="sxs-lookup"><span data-stu-id="24ed8-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="24ed8-104">Talvez você não consiga fazer alterações nas políticas recém-criadas imediatamente; aguarde 4 horas e tente modificar uma política recém-criada novamente.</span><span class="sxs-lookup"><span data-stu-id="24ed8-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="24ed8-105">As políticas de reunião são usadas para controlar os recursos que estão disponíveis para os participantes da reunião para reuniões agendadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="24ed8-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="24ed8-106">Alguns recursos das políticas de reunião podem ainda não ser implementados no centro de administração do Teams (eles são rotulados como "em breve" na documentação).</span><span class="sxs-lookup"><span data-stu-id="24ed8-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="24ed8-107">Nesse caso, ou se você estiver recebendo um erro como "Não podemos atualizar a política agora, mas tentar novamente mais tarde" no Centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar políticas de reunião do Teams.</span><span class="sxs-lookup"><span data-stu-id="24ed8-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="24ed8-108">Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="24ed8-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="24ed8-109">Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, consulte Gerenciar políticas de reunião [no Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="24ed8-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="24ed8-110">Para fazer alterações de política usando cmdlets do PowerShell, consulte [Visão geral do Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="24ed8-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="24ed8-111">Você precisa usar o módulo [do PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) do Skype for Business para políticas de reunião do Teams.</span><span class="sxs-lookup"><span data-stu-id="24ed8-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="24ed8-112">Revise a [documentação dos cmdlets \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="24ed8-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>


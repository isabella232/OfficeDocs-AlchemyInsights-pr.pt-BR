---
title: Gravação de chamada 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696910"
---
# <a name="11-call-recording"></a><span data-ttu-id="21463-102">Gravação de chamada 1:1</span><span class="sxs-lookup"><span data-stu-id="21463-102">1:1 call recording</span></span>

<span data-ttu-id="21463-103">Se o **botão Iniciar Gravação** estiver acinzado em uma chamada 1:1, você precisará alterar as configurações de política do usuário afetado.</span><span class="sxs-lookup"><span data-stu-id="21463-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="21463-104">A partir de 31 de maio de 2021, vamos começar a aplicar uma nova política de chamada Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="21463-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="21463-105">Antes dessa alteração, a gravação de chamada 1:1 é controlada pela Política de Reunião *AllowCloudRecording* Teams Meeting.</span><span class="sxs-lookup"><span data-stu-id="21463-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="21463-106">Essa alteração é documentada na postagem central de mensagens: [(Atualizado) 1:1 Introdução](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)da política de gravação de chamada.</span><span class="sxs-lookup"><span data-stu-id="21463-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="21463-107">*AllowCloudRecordingForCalls*   a opção de política de chamada é definida **como $False** por padrão.</span><span class="sxs-lookup"><span data-stu-id="21463-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="21463-108">Se você preferir impedir que todos os usuários gravam chamadas 1:1, não é necessário tomar nenhuma ação.</span><span class="sxs-lookup"><span data-stu-id="21463-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="21463-109">Para habilitar a gravação de chamadas para todos os usuários em chamadas 1:1, use Teams PowerShell para executar o seguinte cmdlet:</span><span class="sxs-lookup"><span data-stu-id="21463-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="21463-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="21463-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="21463-111">Como alternativa, você pode criar uma nova política e definir  **-AllowCloudRecordingForCalls** para $true e atribuir essa política aos seus usuários.</span><span class="sxs-lookup"><span data-stu-id="21463-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="21463-112">Para obter mais informações, consulte 1:1 Controles de Política de [Gravação de Chamada são (Quase!) Aqui](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="21463-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>

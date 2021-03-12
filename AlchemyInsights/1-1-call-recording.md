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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733837"
---
# <a name="11-call-recording"></a><span data-ttu-id="6d89f-102">Gravação de chamada 1:1</span><span class="sxs-lookup"><span data-stu-id="6d89f-102">1:1 call recording</span></span>

<span data-ttu-id="6d89f-103">Os administradores precisam tomar medidas agora para continuar permitindo que os usuários gravem chamadas 1:1.</span><span class="sxs-lookup"><span data-stu-id="6d89f-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="6d89f-104">A partir de 12 de abril de 2021, vamos começar a impor uma nova opção de Política de Chamada do Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="6d89f-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="6d89f-105">Atualmente, os recursos de gravação de chamada 1:1 são controlados pela *opção AllowCloudRecording* em Políticas de Reunião do Teams.</span><span class="sxs-lookup"><span data-stu-id="6d89f-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="6d89f-106">Se os usuários puderem gravar Reuniões do Teams, eles também poderão gravar chamadas 1:1.</span><span class="sxs-lookup"><span data-stu-id="6d89f-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="6d89f-107">Se você preferir impedir que todos os usuários gravam chamadas 1:1, não é necessário tomar nenhuma ação.</span><span class="sxs-lookup"><span data-stu-id="6d89f-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="6d89f-108">A opção de política de *chamada AllowCloudRecordingForCalls* será $False por padrão.</span><span class="sxs-lookup"><span data-stu-id="6d89f-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="6d89f-109">Essa alteração é documentada na seguinte postagem da Central de Mensagens: [(Atualizado) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Política de gravação de chamada Para definir a Opção de Política de Chamada do Teams, você deve usar o [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="6d89f-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="6d89f-110">Para habilitar o registro de **chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="6d89f-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="6d89f-111">**Para desabilitar o registro de chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="6d89f-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>


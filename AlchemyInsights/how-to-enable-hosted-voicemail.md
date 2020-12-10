---
title: Como habilitar a caixa postal hospedada
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608814"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="be943-102">Como habilitar a caixa postal hospedada</span><span class="sxs-lookup"><span data-stu-id="be943-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="be943-103">Para habilitar a caixa postal, **HostedVoicemail** deve ser definido como $true.</span><span class="sxs-lookup"><span data-stu-id="be943-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="be943-104">A propriedade **HostedVoicemail** no usuário usando o PowerShell remoto (RPS).</span><span class="sxs-lookup"><span data-stu-id="be943-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="be943-105">Para obter mais informações sobre como se conectar ao RPS, confira [visão geral do Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre como se conectar ao RPS.</span><span class="sxs-lookup"><span data-stu-id="be943-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="be943-106">O administrador do teams deve estar conectado ao PowerShell remoto para o Teams.</span><span class="sxs-lookup"><span data-stu-id="be943-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="be943-107">No prompt do PowerShell, o administrador do teams pode executar **set-csuser User@contoso.com-HostedVoiceMail $true** onde o URI SIP é do usuário em questão.</span><span class="sxs-lookup"><span data-stu-id="be943-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="be943-108">As alterações nas políticas podem levar até 24 horas para serem replicadas.</span><span class="sxs-lookup"><span data-stu-id="be943-108">Changes to policies can take up to 24 hours to replicate.</span></span>
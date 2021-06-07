---
title: Gerenciar o registro de webinars
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783136"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="91dec-102">Gerenciar o registro de webinars</span><span class="sxs-lookup"><span data-stu-id="91dec-102">Manage webinar registration</span></span>

<span data-ttu-id="91dec-103">Você gerencia quem pode se registrar nos Webinars do Teams usando os comandos do Powershell do Teams.</span><span class="sxs-lookup"><span data-stu-id="91dec-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="91dec-104">Para instalar o Powershell do Teams, consulte [PowerShell do Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="91dec-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="91dec-105">Por padrão, *WhoCanRegister* está habilitado e definido para **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="91dec-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="91dec-106">Para permitir que qualquer pessoa, incluindo usuários anônimos, se registrem, você deve definir a Política de Reunião para **Todos** usando o Comando do Powershell:</span><span class="sxs-lookup"><span data-stu-id="91dec-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="91dec-107">**Observação**: Se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars.</span><span class="sxs-lookup"><span data-stu-id="91dec-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="91dec-108">Para saber mais e habilitar essa configuração, consulte [Gerenciar configurações de reunião no Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="91dec-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="91dec-109">Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.</span><span class="sxs-lookup"><span data-stu-id="91dec-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="91dec-110">Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="91dec-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="91dec-111">Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="91dec-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>

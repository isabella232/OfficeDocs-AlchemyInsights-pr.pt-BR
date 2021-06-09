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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798632"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="5d115-102">Gerenciar o registro de webinars</span><span class="sxs-lookup"><span data-stu-id="5d115-102">Manage webinar registration</span></span>

<span data-ttu-id="5d115-103">Você gerencia quem pode se registrar nos Webinars do Teams usando os comandos do Powershell do Teams.</span><span class="sxs-lookup"><span data-stu-id="5d115-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="5d115-104">Para instalar o Powershell do Teams, consulte [PowerShell do Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="5d115-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="5d115-105">Por padrão, *WhoCanRegister* está habilitado e definido como **Todos**.</span><span class="sxs-lookup"><span data-stu-id="5d115-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="5d115-106">Se você não vir a opção de permitir o registro de Todos no convite da reunião, execute novamente a configuração de *WhoCanRegister* como Todos e aguarde 24 horas.</span><span class="sxs-lookup"><span data-stu-id="5d115-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="5d115-107">Para executar novamente *WhoCanRegister*, use o comando Windows Powershell:</span><span class="sxs-lookup"><span data-stu-id="5d115-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="5d115-108">**Observação**: Se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars.</span><span class="sxs-lookup"><span data-stu-id="5d115-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="5d115-109">Para saber mais e habilitar essa configuração, consulte [Gerenciar configurações de reunião no Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="5d115-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="5d115-110">Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.</span><span class="sxs-lookup"><span data-stu-id="5d115-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="5d115-111">Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="5d115-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="5d115-112">Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="5d115-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>

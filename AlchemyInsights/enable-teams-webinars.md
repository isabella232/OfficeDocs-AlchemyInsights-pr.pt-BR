---
title: Habilitar os Webinars do Microsoft Teams
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760819"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="6eb72-102">Habilitar os Webinars do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6eb72-102">Enable Teams Webinars</span></span>

<span data-ttu-id="6eb72-103">Webinars estão habilitados por padrão.</span><span class="sxs-lookup"><span data-stu-id="6eb72-103">Webinars are enabled by default.</span></span> <span data-ttu-id="6eb72-104">Você pode gerenciar quem pode agendar e se registrar para os Webinars do Microsoft Teams usando os comandos do PowerShell do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6eb72-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="6eb72-105">Todos os usuários que podem criar uma reunião também podem criar uma reunião webinar.</span><span class="sxs-lookup"><span data-stu-id="6eb72-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="6eb72-106">Se você quer gerenciar quem pode agendar os Webinars do Teams, use *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="6eb72-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="6eb72-107">Por padrão, *WhoCanRegister* está habilitado e definido para **Todos**.</span><span class="sxs-lookup"><span data-stu-id="6eb72-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="6eb72-108">Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.</span><span class="sxs-lookup"><span data-stu-id="6eb72-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="6eb72-109">Para alterar essas configurações, você deve instalar o [PowerShell do Microsoft Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="6eb72-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="6eb72-110">Além disso, as Políticas de Reunião são aplicadas nos Webinars do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6eb72-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="6eb72-111">Por exemplo, se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars.</span><span class="sxs-lookup"><span data-stu-id="6eb72-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="6eb72-112">Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="6eb72-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="6eb72-113">Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="6eb72-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
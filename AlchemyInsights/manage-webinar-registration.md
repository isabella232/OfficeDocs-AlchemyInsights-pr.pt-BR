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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760817"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="2bb6f-102">Gerenciar o registro de webinars</span><span class="sxs-lookup"><span data-stu-id="2bb6f-102">Manage webinar registration</span></span>

<span data-ttu-id="2bb6f-103">Você pode gerenciar quem pode se registrar nos Webinars do Microsoft Teams usando os comandos do PowerShell do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2bb6f-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="2bb6f-104">Por padrão, *WhoCanRegister* está habilitado e definido para **Todos**.</span><span class="sxs-lookup"><span data-stu-id="2bb6f-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="2bb6f-105">Se você deseja desativar o registro da reunião, defina *AllowMeetingRegistration* para **Falso**.</span><span class="sxs-lookup"><span data-stu-id="2bb6f-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="2bb6f-106">Para alterar essas configurações, você deve instalar o [PowerShell do Microsoft Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="2bb6f-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="2bb6f-107">Além disso, as Políticas de Reunião são aplicadas nos Webinars do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2bb6f-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="2bb6f-108">Por exemplo, se o ingresso anônimo estiver desativado nas configurações de reunião, os usuários anônimos não poderão ingressar nos webinars.</span><span class="sxs-lookup"><span data-stu-id="2bb6f-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="2bb6f-109">Para saber mais sobre como configurar quem pode se registrar para webinars, consulte [Configurar quem pode se registrar para webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="2bb6f-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="2bb6f-110">Para obter mais informações sobre as configurações das Listas da Microsoft, consulte [Configurações de controle das Listas da Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="2bb6f-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
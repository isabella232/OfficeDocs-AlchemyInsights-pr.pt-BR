---
title: Ícone de calendário não exibido no cliente do Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819941"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="6e001-102">Ícone de calendário não exibido no cliente do Teams</span><span class="sxs-lookup"><span data-stu-id="6e001-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="6e001-103">A guia Calendário no Teams exige acesso a uma caixa de correio do Exchange através dos Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e001-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="6e001-104">A caixa de correio do Exchange pode ser Online ou Local.</span><span class="sxs-lookup"><span data-stu-id="6e001-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="6e001-105">Para os usuários Online que não veem a guia Calendário, certifique-se de que eles [estejam licenciados para uma caixa de correio do Exchange Online e que a caixa de correio esteja habilitada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="6e001-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="6e001-106">Se o usuário tem uma caixa de correio válida no Exchange Online, mas ainda não consegue ver a guia Calendário, você pode estar enfrentando um problema de rede.</span><span class="sxs-lookup"><span data-stu-id="6e001-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="6e001-107">Use o [Analisador de Conectividade Remota da Microsoft](https://testconnectivity.microsoft.com/) e execute os **Testes de Conectividade dos Serviços Web do Microsoft Exchange** para o usuário afetado.</span><span class="sxs-lookup"><span data-stu-id="6e001-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="6e001-108">Por fim, confira as [Políticas de configuração de aplicativos – aplicativos do Teams](https://admin.teams.microsoft.com/policies/app-setup) para garantir que o aplicativo de Calendário não tenha sido removido da política aplicada ao usuário (provavelmente a **Global (padrão de toda a organização)**.</span><span class="sxs-lookup"><span data-stu-id="6e001-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="6e001-109">Se os usuários estiverem hospedados No Local, você precisa confirmar se a configuração híbrida está íntegra.</span><span class="sxs-lookup"><span data-stu-id="6e001-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="6e001-110">Use o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar problemas.</span><span class="sxs-lookup"><span data-stu-id="6e001-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="6e001-111">Observe que [o Teams exige o Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="6e001-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

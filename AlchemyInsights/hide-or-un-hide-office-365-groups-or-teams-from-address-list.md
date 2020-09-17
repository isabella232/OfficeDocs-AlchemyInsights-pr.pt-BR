---
title: Ocultar ou reexibir grupos ou equipes do Office 365 da lista de endereços
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782315"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="e56f6-102">Ocultar ou reexibir grupos ou equipes do Office 365 da lista de endereços</span><span class="sxs-lookup"><span data-stu-id="e56f6-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="e56f6-103">Use o seguinte comando do EXO PowerShell para ocultar ou ocultar o grupo/equipes do Office 365 das listas de endereços (GAL) dos clientes do Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="e56f6-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="e56f6-104">Use o seguinte comando do EXO PowerShell para ocultar ou ocultar o grupo/equipes do Office365 dos clientes do Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="e56f6-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="e56f6-105">Para obter instruções detalhadas, consulte [Ocultar grupos do Office 365 nos clientes GAL e Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="e56f6-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>

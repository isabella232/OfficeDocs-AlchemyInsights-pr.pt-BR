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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ocultar ou reexibir grupos ou equipes do Office 365 da lista de endereços

Use o seguinte comando do EXO PowerShell para ocultar ou ocultar o grupo/equipes do Office 365 das listas de endereços (GAL) dos clientes do Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Use o seguinte comando do EXO PowerShell para ocultar ou ocultar o grupo/equipes do Office365 dos clientes do Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Para obter instruções detalhadas, consulte [Ocultar grupos do Office 365 nos clientes GAL e Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).

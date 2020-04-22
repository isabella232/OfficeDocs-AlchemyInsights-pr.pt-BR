---
title: Aposentadoria de ferramentas de descoberta eletrônica herdadas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650556"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Aposentadoria de ferramentas de descoberta eletrônica herdadas

Como resultado da nova e aprimorada funcionalidade de descoberta eletrônica no centro de conformidade da Microsoft 365, as seguintes ferramentas e comandos de descoberta eletrônica herdadas serão desativadas nos próximos meses:

- [Descoberta eletrônica in-loco](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [bloqueios in-loco](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no centro de administração do Exchange.

- Os cmdlets do PowerShell do Exchange Online que dão suporte a descoberta eletrônica in-loco e bloqueios in-loco. (Estes cmdlets são identificados coletivamente como cmdlets *-MailboxSearch.) Isso inclui os seguintes cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- O cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) no PowerShell do Exchange Online.
- As operações a seguir na API de serviços Web do Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Descoberta eletrônica avançada v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Linha do tempo para aposentadoria**:
- 1 de abril de 2020: você não poderá criar novas pesquisas e isenções, mas ainda poderá executar, editar e excluir pesquisas existentes de sua responsabilidade. O suporte da Microsoft não oferecerá mais suporte a descoberta eletrônica in-loco & segura no Eat.

- 1º de julho de 2020: o & de descoberta eletrônica in-loco tem funcionalidade no Eat será colocado em um modo somente leitura. Isso significa que você só poderá remover pesquisas e isenções existentes.

**Para obter mais informações, consulte**:

 - [Migrar pesquisas de descoberta eletrônica herdadas e isenções para o centro de conformidade da Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Baixa das ferramentas de Descoberta Eletrônica herdadas](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Perguntas frequentes sobre a descoberta eletrônica in-loco e bloqueios in-loco](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




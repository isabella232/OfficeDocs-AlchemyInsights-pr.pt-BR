---
title: Aposentadoria das Ferramentas de Descoberta Online Herdou
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074633"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Aposentadoria das Ferramentas de Descoberta Online Herdou

Como resultado da funcionalidade de Descoberta Eletrônica nova e aprimorada no centro de Conformidade do Microsoft 365, as seguintes ferramentas e comandos herdados de Descoberta Eletrônica serão retirados nos próximos meses:

- [Descoberta In-loco e](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) retém [in-loco](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no Exchange de administração.

- Os Exchange Online do PowerShell que suportam In-Place Descoberta Eletrônica e In-Place Retém. (Esses cmdlets são identificados coletivamente como cmdlets *-MailboxSearch.) Isso inclui os seguintes cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- O cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) no Exchange Online PowerShell.
- As seguintes operações na API Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Linha do tempo para a aposentadoria**:
- **1º de julho de 2020** Você não pode mais criar novas pesquisas e retém, mas pode executar, editar e excluir pesquisas existentes por sua conta e risco. O Suporte da Microsoft não dá mais suporte In-Place & de Descoberta & no EAC.
    
- 1º de outubro de **2020** In-Place a funcionalidade de & Retém no EAC será colocada no modo somente leitura, portanto, você só pode remover pesquisas e restituições existentes.

**Para obter mais informações, consulte**:

 - [Migrar pesquisas e retê-Centro de conformidade do Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Baixa das ferramentas de Descoberta Eletrônica herdadas](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Perguntas frequentes sobre In-Place eDiscovery e In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




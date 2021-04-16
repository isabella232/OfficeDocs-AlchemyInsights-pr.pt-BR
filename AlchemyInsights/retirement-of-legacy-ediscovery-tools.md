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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798537"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Aposentadoria das Ferramentas de Descoberta Online Herdou

Como resultado da funcionalidade de Descoberta Eletrônica nova e aprimorada no Centro de Conformidade do Microsoft 365, as seguintes ferramentas e comandos herdados de Descoberta Eletrônica serão retirados nos próximos meses:

- [Descoberta In-place e](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) Retém [in-place](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no centro de administração do Exchange.

- Os cmdlets do PowerShell do Exchange Online que suportam In-Place eDiscovery e In-Place Holds. (Esses cmdlets são identificados coletivamente como cmdlets *-MailboxSearch.) Isso inclui os seguintes cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- O cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) no PowerShell do Exchange Online.
- As seguintes operações na API dos Serviços Web do Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Descoberta eDiscoveria Avançada v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Linha do tempo para a aposentadoria**:
- **1º de julho de 2020** Você não pode mais criar novas pesquisas e retém, mas pode executar, editar e excluir pesquisas existentes por sua conta e risco. O Suporte da Microsoft não dá mais suporte In-Place & de Descoberta & no EAC.
    
- 1º de outubro de **2020** In-Place a funcionalidade de & Retém no EAC será colocada no modo somente leitura, portanto, você só pode remover pesquisas e restituições existentes.

**Para obter mais informações, consulte**:

 - [Migrar pesquisas de Descobertas EDiscovery herdado e retê-lo no centro de conformidade do Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Baixa das ferramentas de Descoberta Eletrônica herdadas](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Perguntas frequentes sobre In-Place eDiscovery e In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




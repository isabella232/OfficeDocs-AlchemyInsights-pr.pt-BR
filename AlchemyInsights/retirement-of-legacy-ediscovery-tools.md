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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="f4bb5-102">Aposentadoria das Ferramentas de Descoberta Online Herdou</span><span class="sxs-lookup"><span data-stu-id="f4bb5-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="f4bb5-103">Como resultado da funcionalidade de Descoberta Eletrônica nova e aprimorada no Centro de Conformidade do Microsoft 365, as seguintes ferramentas e comandos herdados de Descoberta Eletrônica serão retirados nos próximos meses:</span><span class="sxs-lookup"><span data-stu-id="f4bb5-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="f4bb5-104">[Descoberta In-place e](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) Retém [in-place](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4bb5-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="f4bb5-105">Os cmdlets do PowerShell do Exchange Online que suportam In-Place eDiscovery e In-Place Holds.</span><span class="sxs-lookup"><span data-stu-id="f4bb5-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="f4bb5-106">(Esses cmdlets são identificados coletivamente como cmdlets \*-MailboxSearch.) Isso inclui os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="f4bb5-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="f4bb5-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f4bb5-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="f4bb5-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f4bb5-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="f4bb5-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f4bb5-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="f4bb5-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f4bb5-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="f4bb5-111">O cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) no PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f4bb5-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="f4bb5-112">As seguintes operações na API dos Serviços Web do Exchange:</span><span class="sxs-lookup"><span data-stu-id="f4bb5-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="f4bb5-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="f4bb5-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="f4bb5-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f4bb5-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="f4bb5-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f4bb5-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="f4bb5-116">Descoberta eDiscoveria Avançada v1.0</span><span class="sxs-lookup"><span data-stu-id="f4bb5-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="f4bb5-117">**Linha do tempo para a aposentadoria**:</span><span class="sxs-lookup"><span data-stu-id="f4bb5-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="f4bb5-118">**1º de julho de 2020** Você não pode mais criar novas pesquisas e retém, mas pode executar, editar e excluir pesquisas existentes por sua conta e risco.</span><span class="sxs-lookup"><span data-stu-id="f4bb5-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="f4bb5-119">O Suporte da Microsoft não dá mais suporte In-Place & de Descoberta & no EAC.</span><span class="sxs-lookup"><span data-stu-id="f4bb5-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="f4bb5-120">1º de outubro de **2020** In-Place a funcionalidade de & Retém no EAC será colocada no modo somente leitura, portanto, você só pode remover pesquisas e restituições existentes.</span><span class="sxs-lookup"><span data-stu-id="f4bb5-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="f4bb5-121">**Para obter mais informações, consulte**:</span><span class="sxs-lookup"><span data-stu-id="f4bb5-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="f4bb5-122">Migrar pesquisas de Descobertas EDiscovery herdado e retê-lo no centro de conformidade do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f4bb5-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="f4bb5-123">Baixa das ferramentas de Descoberta Eletrônica herdadas</span><span class="sxs-lookup"><span data-stu-id="f4bb5-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="f4bb5-124">Perguntas frequentes sobre In-Place eDiscovery e In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="f4bb5-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




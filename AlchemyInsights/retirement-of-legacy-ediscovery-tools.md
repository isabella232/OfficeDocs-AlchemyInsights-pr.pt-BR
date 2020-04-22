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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="81111-102">Aposentadoria de ferramentas de descoberta eletrônica herdadas</span><span class="sxs-lookup"><span data-stu-id="81111-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="81111-103">Como resultado da nova e aprimorada funcionalidade de descoberta eletrônica no centro de conformidade da Microsoft 365, as seguintes ferramentas e comandos de descoberta eletrônica herdadas serão desativadas nos próximos meses:</span><span class="sxs-lookup"><span data-stu-id="81111-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="81111-104">[Descoberta eletrônica in-loco](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [bloqueios in-loco](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="81111-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="81111-105">Os cmdlets do PowerShell do Exchange Online que dão suporte a descoberta eletrônica in-loco e bloqueios in-loco.</span><span class="sxs-lookup"><span data-stu-id="81111-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="81111-106">(Estes cmdlets são identificados coletivamente como cmdlets \*-MailboxSearch.) Isso inclui os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="81111-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="81111-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="81111-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="81111-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="81111-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="81111-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="81111-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="81111-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="81111-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="81111-111">O cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) no PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="81111-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="81111-112">As operações a seguir na API de serviços Web do Exchange:</span><span class="sxs-lookup"><span data-stu-id="81111-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="81111-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="81111-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="81111-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="81111-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="81111-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="81111-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="81111-116">Descoberta eletrônica avançada v 1.0</span><span class="sxs-lookup"><span data-stu-id="81111-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="81111-117">**Linha do tempo para aposentadoria**:</span><span class="sxs-lookup"><span data-stu-id="81111-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="81111-118">1 de abril de 2020: você não poderá criar novas pesquisas e isenções, mas ainda poderá executar, editar e excluir pesquisas existentes de sua responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="81111-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="81111-119">O suporte da Microsoft não oferecerá mais suporte a descoberta eletrônica in-loco & segura no Eat.</span><span class="sxs-lookup"><span data-stu-id="81111-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="81111-120">1º de julho de 2020: o & de descoberta eletrônica in-loco tem funcionalidade no Eat será colocado em um modo somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81111-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="81111-121">Isso significa que você só poderá remover pesquisas e isenções existentes.</span><span class="sxs-lookup"><span data-stu-id="81111-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="81111-122">**Para obter mais informações, consulte**:</span><span class="sxs-lookup"><span data-stu-id="81111-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="81111-123">Migrar pesquisas de descoberta eletrônica herdadas e isenções para o centro de conformidade da Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="81111-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="81111-124">Baixa das ferramentas de Descoberta Eletrônica herdadas</span><span class="sxs-lookup"><span data-stu-id="81111-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="81111-125">Perguntas frequentes sobre a descoberta eletrônica in-loco e bloqueios in-loco</span><span class="sxs-lookup"><span data-stu-id="81111-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




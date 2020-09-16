---
title: Aposentadoria de ferramentas de descoberta eletrônica herdadas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727771"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="67a13-102">Aposentadoria de ferramentas de descoberta eletrônica herdadas</span><span class="sxs-lookup"><span data-stu-id="67a13-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="67a13-103">Como resultado da nova e aprimorada funcionalidade de descoberta eletrônica no centro de conformidade da Microsoft 365, as seguintes ferramentas e comandos de descoberta eletrônica herdadas serão desativadas nos próximos meses:</span><span class="sxs-lookup"><span data-stu-id="67a13-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="67a13-104">[Descoberta eletrônica in-loco](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [bloqueios in-loco](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no centro de administração do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67a13-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="67a13-105">Os cmdlets do PowerShell do Exchange Online que dão suporte a descoberta eletrônica in-loco e bloqueios in-loco.</span><span class="sxs-lookup"><span data-stu-id="67a13-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="67a13-106">(Estes cmdlets são identificados coletivamente como cmdlets \*-MailboxSearch.) Isso inclui os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="67a13-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="67a13-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="67a13-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="67a13-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="67a13-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="67a13-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="67a13-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="67a13-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="67a13-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="67a13-111">O cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) no PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="67a13-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="67a13-112">As operações a seguir na API de serviços Web do Exchange:</span><span class="sxs-lookup"><span data-stu-id="67a13-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="67a13-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="67a13-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="67a13-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="67a13-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="67a13-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="67a13-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="67a13-116">Descoberta eletrônica avançada v 1.0</span><span class="sxs-lookup"><span data-stu-id="67a13-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="67a13-117">**Linha do tempo para aposentadoria**:</span><span class="sxs-lookup"><span data-stu-id="67a13-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="67a13-118">**1º de julho de 2020** Você não pode mais criar novas pesquisas e isenções, mas pode executar, editar e excluir pesquisas existentes de sua responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="67a13-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="67a13-119">O suporte da Microsoft não oferece mais suporte a descoberta eletrônica in-loco & segura no Eat.</span><span class="sxs-lookup"><span data-stu-id="67a13-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="67a13-120">**1 de outubro de 2020** A funcionalidade de descoberta eletrônica in-loco &s no Eat será colocada no modo somente leitura, portanto, você só poderá remover pesquisas e isenções existentes.</span><span class="sxs-lookup"><span data-stu-id="67a13-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="67a13-121">**Para obter mais informações, consulte**:</span><span class="sxs-lookup"><span data-stu-id="67a13-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="67a13-122">Migrar pesquisas de descoberta eletrônica herdadas e isenções para o centro de conformidade da Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="67a13-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="67a13-123">Baixa das ferramentas de Descoberta Eletrônica herdadas</span><span class="sxs-lookup"><span data-stu-id="67a13-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="67a13-124">Perguntas frequentes sobre a descoberta eletrônica in-loco e bloqueios in-loco</span><span class="sxs-lookup"><span data-stu-id="67a13-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




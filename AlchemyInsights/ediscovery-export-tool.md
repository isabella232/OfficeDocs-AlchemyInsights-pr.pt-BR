---
title: Ferramenta de exportação de Descoberta Eletrônica
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814576"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="20412-102">Não é possível instalar ou executar a Ferramenta de Exportação de Descoberta Digital?</span><span class="sxs-lookup"><span data-stu-id="20412-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="20412-103">Se você não puder instalar ou executar a Ferramenta de Exportação de Descoberta Digital para baixar os resultados da pesquisa, verifique as seguintes coisas:</span><span class="sxs-lookup"><span data-stu-id="20412-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="20412-104">O computador que você está usando atende a esses pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="20412-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="20412-105">Versões de 32 e 64 bits do Windows 7 e versões posteriores</span><span class="sxs-lookup"><span data-stu-id="20412-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="20412-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="20412-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="20412-107">Um navegador com suporte:</span><span class="sxs-lookup"><span data-stu-id="20412-107">A supported browser:</span></span>

  - <span data-ttu-id="20412-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="20412-108">Microsoft Edge</span></span>

    <span data-ttu-id="20412-109">Ou</span><span class="sxs-lookup"><span data-stu-id="20412-109">Or</span></span>

  - <span data-ttu-id="20412-110">Internet Explorer 10 e versões posteriores</span><span class="sxs-lookup"><span data-stu-id="20412-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="20412-111">Não há suporte para outros navegadores, como o Google Chrome e o Mozilla Firefox.</span><span class="sxs-lookup"><span data-stu-id="20412-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="20412-112">Sua organização pode se conectar ao ponto de extremidade no Azure, que é **\* .blob.core.windows.net** (o curinga representa um identificador exclusivo para seu trabalho de exportação).</span><span class="sxs-lookup"><span data-stu-id="20412-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="20412-113">Você recebe a função Exportar no Centro de Conformidade de Segurança do Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="20412-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="20412-114">Por padrão, essa função é atribuída apenas ao grupo de funções do Gerenciador de Descobertas.</span><span class="sxs-lookup"><span data-stu-id="20412-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="20412-115">Consulte [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="20412-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="20412-116">Para obter mais informações, consulte [Exportar resultados da Pesquisa de Conteúdo](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="20412-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="20412-117">Se você estiver exportando mais de 100.000 caixas de correio, você precisará usar o Powershell a seguir para baixar os resultados de Exportação: Exportando resultados de mais de  [100.000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)caixas de correio .</span><span class="sxs-lookup"><span data-stu-id="20412-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
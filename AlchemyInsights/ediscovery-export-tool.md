---
title: Ferramenta de exportação de Descoberta Eletrônica
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277949"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="e37d7-102">Não é possível instalar ou executar a ferramenta de exportação de descoberta eletrônica?</span><span class="sxs-lookup"><span data-stu-id="e37d7-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="e37d7-103">Se você não conseguir instalar ou executar a ferramenta de exportação de descoberta eletrônica para baixar os resultados da pesquisa, verifique as seguintes coisas:</span><span class="sxs-lookup"><span data-stu-id="e37d7-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="e37d7-104">O computador que você está usando atende a esses pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="e37d7-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="e37d7-105">Versões de 32 e 64 bits do Windows 7 e versões posteriores</span><span class="sxs-lookup"><span data-stu-id="e37d7-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="e37d7-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="e37d7-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="e37d7-107">Um navegador com suporte:</span><span class="sxs-lookup"><span data-stu-id="e37d7-107">A supported browser:</span></span>

  - <span data-ttu-id="e37d7-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e37d7-108">Microsoft Edge</span></span>

    <span data-ttu-id="e37d7-109">Ou</span><span class="sxs-lookup"><span data-stu-id="e37d7-109">Or</span></span>

  - <span data-ttu-id="e37d7-110">Internet Explorer 10 e versões posteriores</span><span class="sxs-lookup"><span data-stu-id="e37d7-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="e37d7-111">Outros navegadores, como Google Chrome e Mozilla Firefox, não são suportados.</span><span class="sxs-lookup"><span data-stu-id="e37d7-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="e37d7-112">Sua organização pode se conectar ao ponto de extremidade no Azure, que é \*\* \* . blob.Core.Windows.net\*\* (o caractere curinga representa um identificador exclusivo para seu trabalho de exportação).</span><span class="sxs-lookup"><span data-stu-id="e37d7-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="e37d7-113">Você é atribuído à função exportar no centro de conformidade de segurança do Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="e37d7-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="e37d7-114">Por padrão, essa função só é atribuída ao grupo de função Gerenciador de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="e37d7-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="e37d7-115">Consulte [atribuir permissões de descoberta eletrônica](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="e37d7-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="e37d7-116">Para obter mais informações, consulte [Exportar resultados de pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="e37d7-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="e37d7-117">Se você estiver exportando mais de 100.000 caixas de correio, será necessário usar o seguinte PowerShell para baixar os resultados da exportação:  [exportação de resultados de mais de 100.000 caixas de correio](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="e37d7-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
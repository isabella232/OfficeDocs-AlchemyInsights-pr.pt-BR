---
title: igual ao nome do arquivo é melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683837"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="dbb8b-102">Cabeçalho Alchemy necessário H1, H2's não funcionam.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="dbb8b-103">Práticas recomendadas e diretrizes para a criação de Alchemy:</span><span class="sxs-lookup"><span data-stu-id="dbb8b-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="dbb8b-104">**Não aninhe Alchemy insights em Folders**: isso quebrará a estrutura da URL.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="dbb8b-105">Estamos tentando corrigir isso.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="dbb8b-106">Os arquivos na pasta **AlchemyInsights** devem ter nomes de arquivo em minúsculas com hifens para espaços por exemplo.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="dbb8b-107">***How-to-Enable-litígio-Hold***.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="dbb8b-108">Inclua a ID de regra ou a ID de Bucket do [portal do parceiro Alchemy](https://alchemyportal.azurewebsites.net) no campo MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="dbb8b-109">ex.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-109">ex.</span></span> <span data-ttu-id="dbb8b-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="dbb8b-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="dbb8b-111">Use o restante dos metadados na parte superior do arquivo como modelo.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="dbb8b-112">No [portal do parceiro do Alchemy](https://alchemyportal.azurewebsites.net), navegue até a seção **título do atendimento ao cliente:** e use-o como ponto de partida para o título H1 da visão.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="dbb8b-113">O Alchemy insights deve ter apenas um único H1 na parte superior ou eles serão quebrados na produção.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="dbb8b-114">H2S não renderizar use **negrito** ou outras convenções para indicar seções separadas.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="dbb8b-115">Em seguida, preencha o corpo de texto usando o material de rascunho na seção do cliente ideias da página de regra Alchemy</span><span class="sxs-lookup"><span data-stu-id="dbb8b-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="dbb8b-116">Listas com marcadores são boas</span><span class="sxs-lookup"><span data-stu-id="dbb8b-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="dbb8b-117">Listas numeradas muito</span><span class="sxs-lookup"><span data-stu-id="dbb8b-117">Numbered lists too</span></span>
    1. <span data-ttu-id="dbb8b-118">**Negrito** e *itálico* são a-ok</span><span class="sxs-lookup"><span data-stu-id="dbb8b-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="dbb8b-119">Os links devem ser sempre **"links para a Web"/External** ou **links de profundidade para elementos da interface do usuário**, não para links internos.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="dbb8b-120">As imagens não são oficialmente suportadas no momento, mas estão no roteiro.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="dbb8b-121">E isso já é um pouco longo demais.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-121">And this is really already a bit too long.</span></span> <span data-ttu-id="dbb8b-122">A prática recomendada é de cerca de 400 caracteres---------------------------------</span><span class="sxs-lookup"><span data-stu-id="dbb8b-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="dbb8b-123">Depois que o conteúdo estiver pronto, puxe-o para o Live Branch.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="dbb8b-124">Em seguida, vá para o [portal do parceiro Alchemy](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo URL.</span><span class="sxs-lookup"><span data-stu-id="dbb8b-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="dbb8b-125">M</span><span class="sxs-lookup"><span data-stu-id="dbb8b-125">M</span></span>
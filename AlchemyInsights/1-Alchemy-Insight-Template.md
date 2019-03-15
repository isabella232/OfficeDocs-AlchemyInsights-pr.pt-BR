---
title: 'igual ao nome do arquivo é melhor [regra #-Descrição]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634492"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="62328-102">Cabeçalho Alchemy necessário H1, H2's não funcionam.</span><span class="sxs-lookup"><span data-stu-id="62328-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="62328-103">Práticas recomendadas e diretrizes para a criação de Alchemy:</span><span class="sxs-lookup"><span data-stu-id="62328-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="62328-104">**Não aninhe Alchemy insights em Folders**: isso quebrará a estrutura da URL.</span><span class="sxs-lookup"><span data-stu-id="62328-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="62328-105">Estamos tentando corrigir isso.</span><span class="sxs-lookup"><span data-stu-id="62328-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="62328-106">Os arquivos na pasta **AlchemyInsights** devem ter ID de regra e nome de regra do [portal de parceiro do Alchemy](https://alchemyportal.azurewebsites.net) no nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="62328-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="62328-107">ex.</span><span class="sxs-lookup"><span data-stu-id="62328-107">ex.</span></span> <span data-ttu-id="62328-108">***976-instruções-Enable-litígio-retenção***</span><span class="sxs-lookup"><span data-stu-id="62328-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="62328-109">Use os metadados na parte superior desse arquivo como modelo.</span><span class="sxs-lookup"><span data-stu-id="62328-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="62328-110">Nada mais é necessário.</span><span class="sxs-lookup"><span data-stu-id="62328-110">Nothing else is required.</span></span>
1. <span data-ttu-id="62328-111">No [portal do parceiro do Alchemy](https://alchemyportal.azurewebsites.net), navegue até a seção **título do atendimento ao cliente:** e use-o como ponto de partida para o título H1 da visão.</span><span class="sxs-lookup"><span data-stu-id="62328-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="62328-112">O Alchemy insights deve ter apenas um único H1 na parte superior ou eles serão quebrados na produção.</span><span class="sxs-lookup"><span data-stu-id="62328-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="62328-113">H2S não renderizar use **negrito** ou outras convenções para indicar seções separadas.</span><span class="sxs-lookup"><span data-stu-id="62328-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="62328-114">Em seguida, preencha o corpo de texto usando o material de rascunho na seção do cliente ideias da página de regra Alchemy</span><span class="sxs-lookup"><span data-stu-id="62328-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="62328-115">Listas com marcadores são boas</span><span class="sxs-lookup"><span data-stu-id="62328-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="62328-116">Listas numeradas muito</span><span class="sxs-lookup"><span data-stu-id="62328-116">Numbered lists too</span></span>
    1. <span data-ttu-id="62328-117">**Negrito** e *itálico* são a-ok</span><span class="sxs-lookup"><span data-stu-id="62328-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="62328-118">Os links devem ser sempre **"links para a Web"/External** ou **links de profundidade para elementos da interface do usuário**, não para links internos.</span><span class="sxs-lookup"><span data-stu-id="62328-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="62328-119">E isso já é um pouco longo demais.</span><span class="sxs-lookup"><span data-stu-id="62328-119">And this is really already a bit too long.</span></span> <span data-ttu-id="62328-120">A prática recomendada é de cerca de 400 caracteres---------------------------------</span><span class="sxs-lookup"><span data-stu-id="62328-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="62328-121">Depois que o conteúdo estiver pronto, puxe-o para o Live Branch.</span><span class="sxs-lookup"><span data-stu-id="62328-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="62328-122">Em seguida, vá para o [portal do parceiro Alchemy](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo URL.</span><span class="sxs-lookup"><span data-stu-id="62328-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="62328-123">Verifique se as informações revisadas e publicadas diz "Sim" e clique em atualizar regra.</span><span class="sxs-lookup"><span data-stu-id="62328-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="62328-124">**(Isso será prettier na nova versão do portal-lançamento em breve.)** 
 ![campo URL](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="62328-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>


---
title: 'é igual ao nome de arquivo é melhor [regra #-descrição]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697118"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="a8480-102">Obrigatório Alquimia cabeçalho S1, S2 não funcionam.</span><span class="sxs-lookup"><span data-stu-id="a8480-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="a8480-103">Práticas recomendadas e diretrizes para a criação de Alquimia:</span><span class="sxs-lookup"><span data-stu-id="a8480-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="a8480-p101">**Não aninhar Alquimia ideias de pesquisas nas pastas**- Isso interromperá a estrutura da url. Estamos analisando corrigindo isso.</span><span class="sxs-lookup"><span data-stu-id="a8480-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="a8480-106">Arquivos na pasta **AlchemyInsights** devem ter o ID da regra e o nome da regra a partir do [portal Alquimia parceiro](https://alchemyportal.azurewebsites.net) no nome de arquivo.</span><span class="sxs-lookup"><span data-stu-id="a8480-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="a8480-p102">***976-How-to-enable-litigation-hold*** ex.</span><span class="sxs-lookup"><span data-stu-id="a8480-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="a8480-p103">Use os metadados na parte superior desse arquivo como seu modelo. Nada mais é necessário.</span><span class="sxs-lookup"><span data-stu-id="a8480-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="a8480-111">No [portal Alquimia parceiro](https://alchemyportal.azurewebsites.net), navegue até a seção **título percepção de cliente:** e usá-la como uma partida aponte para seu título S1 para o insight.</span><span class="sxs-lookup"><span data-stu-id="a8480-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="a8480-p104">Ideias de Alquimia deve ter apenas um único S1 na parte superior ou eles serão interrompidos em produção. H2s não processar afirmativo usar **negrito** ou outras convenções para significar seções separadas.</span><span class="sxs-lookup"><span data-stu-id="a8480-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="a8480-114">Em seguida, preencha o corpo de texto usando o material de rascunho na seção ideias dos clientes da página Alquimia regra</span><span class="sxs-lookup"><span data-stu-id="a8480-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="a8480-115">Listas com marcadores são finas</span><span class="sxs-lookup"><span data-stu-id="a8480-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="a8480-116">Muito de listas numeradas</span><span class="sxs-lookup"><span data-stu-id="a8480-116">Numbered lists too</span></span>
    1. <span data-ttu-id="a8480-117">**Negrito** e *itálico* são a-ok</span><span class="sxs-lookup"><span data-stu-id="a8480-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="a8480-118">Links sempre deve ser um **"links web" / externo** OR **profunda-links para os elementos de interface do usuário**, os links não internos.</span><span class="sxs-lookup"><span data-stu-id="a8480-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="a8480-p105">E isso realmente já é um pouco muito longo. Prática recomendada é aproximadamente 400 caracteres--</span><span class="sxs-lookup"><span data-stu-id="a8480-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="a8480-p106">Depois que o conteúdo está pronto, retire-o à ramificação ao vivo. Em seguida, vá para o [portal de parceiros Alquimia](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo url. Certifique-se de Insight revisado e publicado diz "Sim" e clique em regra de atualização. **(Isso terá uma aparência mais bonito na nova versão do portal - liberando em breve.)** 
 ![campo url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="a8480-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>


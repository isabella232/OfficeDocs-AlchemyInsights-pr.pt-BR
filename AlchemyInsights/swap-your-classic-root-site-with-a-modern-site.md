---
title: Trocar o site da raiz clássica por um site moderno
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245915"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="38e62-102">Trocar o site da raiz clássica por um site moderno</span><span class="sxs-lookup"><span data-stu-id="38e62-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="38e62-103">Se seu ambiente tiver sido configurado antes de abril de 2019, você poderá alterar seu site raiz para um site moderno usando o Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="38e62-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="38e62-104">Se você tiver um site diferente que você deseja usar como seu site raiz, você pode substituir (trocar) o site raiz por ele.</span><span class="sxs-lookup"><span data-stu-id="38e62-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="38e62-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site com outro site enquanto arquiva o site original.</span><span class="sxs-lookup"><span data-stu-id="38e62-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="38e62-106">Disponível para o site de equipe (não conectado a um grupo) e site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="38e62-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="38e62-107">Recursos adicionais serão introduzidos em breve, permitindo que você continue usando o conteúdo do site, mas converta o site existente em um site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="38e62-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="38e62-108">Esses recursos serão implantados gradualmente.</span><span class="sxs-lookup"><span data-stu-id="38e62-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="38e62-109">Continue a verificar o centro de mensagens do Office 365 para atualizações.</span><span class="sxs-lookup"><span data-stu-id="38e62-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="38e62-110">Problemas conhecidos com o swap de sites</span><span class="sxs-lookup"><span data-stu-id="38e62-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="38e62-111">O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="38e62-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="38e62-112">O conteúdo deverá ser rastreado para atualizar o índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="38e62-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="38e62-113">Não há nenhuma etapa manual necessária-isso será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="38e62-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="38e62-114">Qualquer coisa dependente de links "estáticos" (como sincronização de arquivos e arquivos do OneNote) precisará ser corrigida manualmente.</span><span class="sxs-lookup"><span data-stu-id="38e62-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="38e62-115">Se o site de origem for um site de notícias organizacionais, atualize a URL.</span><span class="sxs-lookup"><span data-stu-id="38e62-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="38e62-116">Obtenha uma lista de todos os sites de notícias organizacionais.</span><span class="sxs-lookup"><span data-stu-id="38e62-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="38e62-117">Talvez seja necessário validar os sites do Project Server para garantir que eles ainda estejam associados corretamente.</span><span class="sxs-lookup"><span data-stu-id="38e62-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>






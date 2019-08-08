---
title: Site moderno como o site raiz
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232703"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="af087-102">Site moderno como site raiz</span><span class="sxs-lookup"><span data-stu-id="af087-102">Modern site as root site</span></span>

<span data-ttu-id="af087-103">Começamos a implementar um novo recurso que permitirá trocar seu site de raiz de site clássico por um site moderno.</span><span class="sxs-lookup"><span data-stu-id="af087-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="af087-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site com outro site enquanto arquiva o site original.</span><span class="sxs-lookup"><span data-stu-id="af087-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="af087-105">Disponível para o site de equipe (não conectado a um grupo) e site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="af087-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="af087-106">Não exclua o site da raiz clássica para criar um site de comunicação moderno.</span><span class="sxs-lookup"><span data-stu-id="af087-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="af087-107">Isso não é suportado pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="af087-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="af087-108">A exclusão do site raiz tornará todos os sites do SharePoint em sua organização inacessíveis a todos os usuários, até que você restaure o site ou crie um novo site na mesma URL.</span><span class="sxs-lookup"><span data-stu-id="af087-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="af087-109">Vamos comunicar esse recurso por meio do centro de mensagens.</span><span class="sxs-lookup"><span data-stu-id="af087-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="af087-110">Você deve esperar que o recurso seja ativado em seu locatário em breve.</span><span class="sxs-lookup"><span data-stu-id="af087-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="af087-111">Problemas conhecidos com o swap de sites</span><span class="sxs-lookup"><span data-stu-id="af087-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="af087-112">O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="af087-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="af087-113">O conteúdo deverá ser rastreado para atualizar o índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="af087-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="af087-114">Não é necessária nenhuma etapa manual aqui, isso será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="af087-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="af087-115">Qualquer coisa dependente de links "estáticos" (como sincronização de arquivos e arquivos do OneNote) precisará ser corrigida manualmente.</span><span class="sxs-lookup"><span data-stu-id="af087-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="af087-116">Talvez seja necessário validar os sites do Project Server para garantir que eles ainda estejam associados corretamente.</span><span class="sxs-lookup"><span data-stu-id="af087-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 

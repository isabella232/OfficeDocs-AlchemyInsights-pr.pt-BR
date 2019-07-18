---
title: Dynamics 365-apresentações de painel incorretas na interface unificada do Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35746869"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="8f9bd-102">Apresentações de painel incorretas na interface unificada do Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="8f9bd-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="8f9bd-103">Há várias razões pelas quais você pode ver um painel diferente do que você espera:</span><span class="sxs-lookup"><span data-stu-id="8f9bd-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="8f9bd-104">O usuário configurou um painel de usuário padrão</span><span class="sxs-lookup"><span data-stu-id="8f9bd-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="8f9bd-105">Normalmente, você pode identificar um painel padrão do usuário é definido se o botão **definir como padrão** não for exibido na barra de comandos do painel.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="8f9bd-106">O painel padrão do usuário substituirá todos os outros painéis padrão, mesmo que o painel padrão do usuário não esteja no aplicativo atual.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="8f9bd-107">Use a seguinte solução alternativa para remover o painel padrão.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="8f9bd-108">Criar um novo painel pessoal.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="8f9bd-109">Defina esse novo painel como o usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="8f9bd-110">Exclua esse painel.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="8f9bd-111">O painel é definido no sitemap</span><span class="sxs-lookup"><span data-stu-id="8f9bd-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="8f9bd-112">Você pode ter definido um painel padrão da organização selecionando um painel e escolhendo ' definir como padrão ' em ' Personalizar o sistema '.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="8f9bd-113">Mas o painel definido no designer de sitemap prevalecerá sobre esse painel, se o usuário tiver acesso a ele.</span><span class="sxs-lookup"><span data-stu-id="8f9bd-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="8f9bd-114">Para que os usuários vejam o painel definido como o padrão da organização, você pode:</span><span class="sxs-lookup"><span data-stu-id="8f9bd-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="8f9bd-115">Definir esse painel no sitemap</span><span class="sxs-lookup"><span data-stu-id="8f9bd-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="8f9bd-116">Remover o acesso ao painel definido de sitemap para esses usuários</span><span class="sxs-lookup"><span data-stu-id="8f9bd-116">Remove access to the sitemap defined dashboard for those users</span></span>
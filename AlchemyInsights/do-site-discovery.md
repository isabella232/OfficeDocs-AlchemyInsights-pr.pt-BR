---
title: Fazer descoberta do site
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529157"
---
# <a name="do-site-discovery"></a><span data-ttu-id="74c60-102">Fazer descoberta do site</span><span class="sxs-lookup"><span data-stu-id="74c60-102">Do site discovery</span></span>

<span data-ttu-id="74c60-103">Se a sua organização ainda usa aplicativos da web legados e planeja usar o modo Internet Explorer (o que a maioria dos clientes faz), você deve fazer algumas descobertas de sites adicionais.</span><span class="sxs-lookup"><span data-stu-id="74c60-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="74c60-104">**Você já implantou uma versão mais antiga do Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="74c60-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="74c60-105">Se você já configurou sua Lista de Sites da Empresa para funcionar com a versão herdada do Microsoft Edge, a descoberta de seu site está quase concluída.</span><span class="sxs-lookup"><span data-stu-id="74c60-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="74c60-106">A única coisa que você precisa fazer é adicionar sites neutros.</span><span class="sxs-lookup"><span data-stu-id="74c60-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="74c60-107">Sites neutros são normalmente sites que fornecem logon único (SSO).</span><span class="sxs-lookup"><span data-stu-id="74c60-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="74c60-108">Se você for a um site neutro do Microsoft Edge, deseja permanecer no Microsoft Edge para fazer a autenticação.</span><span class="sxs-lookup"><span data-stu-id="74c60-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="74c60-109">Se você for para um site neutro no modo Internet Explorer, deverá permanecer no modo Internet Explorer para fazer a autenticação.</span><span class="sxs-lookup"><span data-stu-id="74c60-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="74c60-110">Identifique qualquer SSO ou outros sites neutros que você usa e adicione-os à sua Lista de Sites da Empresa.</span><span class="sxs-lookup"><span data-stu-id="74c60-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="74c60-111">**Internet Explorer é o seu navegador padrão**</span><span class="sxs-lookup"><span data-stu-id="74c60-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="74c60-112">Se você estiver usando apenas o Internet Explorer agora, talvez não saiba quais sites foram atualizados para os padrões modernos da web e quais ainda exigem o Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="74c60-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="74c60-113">Você desejará localizar e adicionar esses sites à Lista de Sites da Empresa para que possa usar o modo Internet Explorer apenas para esses sites.</span><span class="sxs-lookup"><span data-stu-id="74c60-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="74c60-114">[A Descoberta de Sites da Empresa](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) descobre sites que podem precisar do modo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="74c60-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="74c60-115">Ele pode coletar dados em computadores que executam o Windows Internet Explorer 8 por meio do Internet Explorer 11 no Windows 10, Windows 8.1 ou Windows 7.</span><span class="sxs-lookup"><span data-stu-id="74c60-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="74c60-116">**Analisar os dados**</span><span class="sxs-lookup"><span data-stu-id="74c60-116">**Analyze the data**</span></span>

<span data-ttu-id="74c60-117">Depois de coletar os dados do site, recomendamos o seguinte processo de quatro etapas para analisar os dados:</span><span class="sxs-lookup"><span data-stu-id="74c60-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="74c60-118">Classifique os dados por domínio e, em seguida, por URL.</span><span class="sxs-lookup"><span data-stu-id="74c60-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="74c60-119">Defina os limites de um aplicativo a ser configurado para o modo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="74c60-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="74c60-120">Você deseja incluir todos os sites e controles da web que definem o aplicativo, mas não deseja incluir sites e controles extras.</span><span class="sxs-lookup"><span data-stu-id="74c60-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="74c60-121">Alguns sites podem ser tão simples como o *https://contoso.com/app1* enquanto outros podem exigir que você defina vários sites e páginas.</span><span class="sxs-lookup"><span data-stu-id="74c60-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="74c60-122">Teste o aplicativo para verificar se ele não funciona nativamente.</span><span class="sxs-lookup"><span data-stu-id="74c60-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="74c60-123">Muitos sites oferecem conteúdo moderno quando detectam um navegador moderno e só oferecem conteúdo legado quando detectam o Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="74c60-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="74c60-124">Adicione o aplicativo à sua Lista de Sites de Empresas se ele falhar no teste.</span><span class="sxs-lookup"><span data-stu-id="74c60-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="74c60-125">Como prática recomendada, agrupe todos os sites que compõem um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c60-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="74c60-126">Dessa forma, quando você atualiza um aplicativo, é mais fácil remover todo o site do modo Internet Explorer e começar a usar um navegador moderno para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c60-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="74c60-127">Depois de concluir a descoberta do site e analisar os dados, você está pronto para começar a analisar sua estratégia de canal.</span><span class="sxs-lookup"><span data-stu-id="74c60-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>


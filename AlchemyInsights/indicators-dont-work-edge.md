---
title: Os indicadores não funcionam com o navegador Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651473"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="73678-102">Os indicadores não funcionam com o navegador Edge</span><span class="sxs-lookup"><span data-stu-id="73678-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="73678-103">Depois de criar um indicador, ele não é respeitado pelo Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="73678-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="73678-104">Para obter mais informações, confira [Criar indicadores para IPs e URLs/domínios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="73678-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="73678-105">Etapa 1: certifique-se do seguinte</span><span class="sxs-lookup"><span data-stu-id="73678-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="73678-106">Verifique se o indicador está correto (sem erros de digitação no IP/URL, ação correta, os grupos RBAC corretos).</span><span class="sxs-lookup"><span data-stu-id="73678-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="73678-107">Aguarde no mínimo 2 horas após a criação do indicador para levar em consideração qualquer latência possível.</span><span class="sxs-lookup"><span data-stu-id="73678-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="73678-108">Confirme se os sistemas estão integrados ao Microsoft Defender para Ponto de Extremidade.</span><span class="sxs-lookup"><span data-stu-id="73678-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="73678-109">Verifique se o(s) sistema(s) podem se comunicar com a nuvem.</span><span class="sxs-lookup"><span data-stu-id="73678-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="73678-110">Verifique se o Smartscreen está habilitado e acessível acessando o [site de teste](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="73678-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="73678-111">Etapa 2: solucionar o problema potencial</span><span class="sxs-lookup"><span data-stu-id="73678-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="73678-112">Certifique-se de que o cliente atende aos requisitos.</span><span class="sxs-lookup"><span data-stu-id="73678-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="73678-113">Para obter detalhes, confira [Criar indicadores para IPs e URLs/domínios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="73678-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="73678-114">Certifique-se de que está executando a versão mais recente do navegador Edge.</span><span class="sxs-lookup"><span data-stu-id="73678-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="73678-115">Para descobrir a versão mais recente, confira [Descubra qual versão do Microsoft Edge você possui](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="73678-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="73678-116">Reinicie o navegador Edge.</span><span class="sxs-lookup"><span data-stu-id="73678-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="73678-117">Navegue até o site para o qual você configurou um indicador.</span><span class="sxs-lookup"><span data-stu-id="73678-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="73678-118">Se o site não aparecer conforme o esperado, vá para a Etapa 3.</span><span class="sxs-lookup"><span data-stu-id="73678-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="73678-119">Etapa 3: coletar dados</span><span class="sxs-lookup"><span data-stu-id="73678-119">Step 3: Collect data</span></span>

- <span data-ttu-id="73678-120">Colete dados de diagnóstico **MDEClientAnalyzer**.</span><span class="sxs-lookup"><span data-stu-id="73678-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="73678-121">Para obter instruções, confira [Problemas com máquinas integradas ao Microsoft Defender para Ponto de Extremidade](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="73678-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="73678-122">Se você se sentir confortável em instalar e coletar um rastreio do Fiddler, confira [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="73678-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="73678-123">Se você preferir orientação do Suporte da Microsoft, selecione o ícone Suporte abaixo para abrir um caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="73678-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>

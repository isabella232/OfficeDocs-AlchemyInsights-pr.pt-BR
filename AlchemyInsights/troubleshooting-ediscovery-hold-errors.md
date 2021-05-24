---
title: Solucionar problemas de erros de suspensão da Descoberta Eletrônica
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583747"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="3a89a-102">Solucionar problemas de erros de suspensão da Descoberta Eletrônica</span><span class="sxs-lookup"><span data-stu-id="3a89a-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="3a89a-103">Enfrentando problemas de suspensão da Descoberta Eletrônica?</span><span class="sxs-lookup"><span data-stu-id="3a89a-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="3a89a-104">Considere uma das seguintes práticas recomendadas:</span><span class="sxs-lookup"><span data-stu-id="3a89a-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="3a89a-105">Verifique o status de distribuição da suspensão.</span><span class="sxs-lookup"><span data-stu-id="3a89a-105">Check the hold distribution status.</span></span>  <span data-ttu-id="3a89a-106">Se o status estiver **Ativado (Pendente)** ou **Desativado (Pendente)**, aguarde a distribuição de suspensão ser concluída.</span><span class="sxs-lookup"><span data-stu-id="3a89a-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="3a89a-107">Mescle as atualizações de suspensão da Descoberta Eletrônica em uma única solicitação em massa, ao invés de atualizar a política repetidamente para cada transação.</span><span class="sxs-lookup"><span data-stu-id="3a89a-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="3a89a-108">Execute Set-CaseHoldPolicy <policyname> –RetryDistribution no Centro de Conformidade e Segurança do Powershell.</span><span class="sxs-lookup"><span data-stu-id="3a89a-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="3a89a-109">Para mais detalhes, confira [Conectar-se ao Centro de Conformidade e Segurança do PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="3a89a-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="3a89a-110">Para obter as etapas de verificação dessas configurações e as práticas recomendadas adicionais para reduzir e resolver problemas de suspensão da Descoberta Eletrônica, confira [Solucionar problemas de erros de suspensão da Descoberta Eletrônica](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="3a89a-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="3a89a-111">Para obter informações sobre como solucionar outros problemas comuns da Descoberta Eletrônica, confira [Investigar e solucionar os problemas mais comuns da Descoberta Eletrônica](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="3a89a-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>

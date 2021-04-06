---
title: Identificar problemas da Área de Trabalho Virtual do Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590259"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="5b554-102">Identificar problemas da Área de Trabalho Virtual do Windows</span><span class="sxs-lookup"><span data-stu-id="5b554-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="5b554-103">O Diagnóstico da Área de Trabalho Virtual do Windows usa apenas um cmdlet do PowerShell, mas contém vários parâmetros opcionais para ajudar a reduzir e isolar problemas.</span><span class="sxs-lookup"><span data-stu-id="5b554-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="5b554-104">Para começar:</span><span class="sxs-lookup"><span data-stu-id="5b554-104">To get started:</span></span> 

1. <span data-ttu-id="5b554-105">Baixe e importe o módulo do PowerShell da Área de Trabalho Virtual do Windows.</span><span class="sxs-lookup"><span data-stu-id="5b554-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="5b554-106">Para obter detalhes, confira [Cmdlets da Área de Trabalho Virtual do Windows para o Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="5b554-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="5b554-107">Execute o cmdlet a seguir para entrar em sua conta:</span><span class="sxs-lookup"><span data-stu-id="5b554-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="5b554-108">Exemplo: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="5b554-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="5b554-109">**OBSERVAÇÃO:** todas as consultas que usam o PowerShell devem incluir os parâmetros -UserName ou -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="5b554-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="5b554-110">Para saber mais sobre recursos de monitoramento, confira [Análise de logs para o recurso de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="5b554-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="5b554-111">Para filtrar as atividades de diagnóstico por usuário, execute o seguinte cmdlet:</span><span class="sxs-lookup"><span data-stu-id="5b554-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="5b554-112">Exemplo: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="5b554-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="5b554-113">Há uma lista de filtros que você pode executar para diagnosticar problemas.</span><span class="sxs-lookup"><span data-stu-id="5b554-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="5b554-114">Para saber mais sobre problemas de diagnóstico, confira [Identificar e diagnosticar problemas da Área de Trabalho Virtual do Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="5b554-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="5b554-115">Para saber mais sobre erros comuns, confira [Cenários de erros comuns](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="5b554-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>

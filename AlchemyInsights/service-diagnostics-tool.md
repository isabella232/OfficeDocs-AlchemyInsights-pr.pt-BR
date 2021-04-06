---
title: Ferramenta de diagnóstico de serviço para Área de Trabalho Virtual do Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590260"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="6307a-102">Ferramenta de diagnóstico de serviço para Área de Trabalho Virtual do Windows</span><span class="sxs-lookup"><span data-stu-id="6307a-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="6307a-103">A Área de Trabalho Virtual do Windows (WVD) oferece uma ferramenta de diagnóstico que permite aos administradores identificar erros por meio de uma única interface.</span><span class="sxs-lookup"><span data-stu-id="6307a-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="6307a-104">Esta ferramenta registra informações relacionadas a diagnósticos sempre que a WVD for utilizada por alguém a quem foi atribuído uma função WVD.</span><span class="sxs-lookup"><span data-stu-id="6307a-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="6307a-105">Cada log contém informações sobre a função WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e as informações sobre o locatário e o usuário.</span><span class="sxs-lookup"><span data-stu-id="6307a-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="6307a-106">A Análise de Log do Azure pode ser configurada para capturar o log de atividades criado pela ferramenta de diagnóstico seguindo estas etapas:</span><span class="sxs-lookup"><span data-stu-id="6307a-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="6307a-107">Crie um espaço de trabalho de Análise de Log com o [portal do Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="6307a-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="6307a-108">[Conectar computadores Windows ao Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="6307a-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="6307a-109">Obtenha a ID do espaço de trabalho e a chave primária de seu espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6307a-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="6307a-110">O assistente de configuração precisa destas informações para configurar corretamente o agente e garantir que ele possa se comunicar com o Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="6307a-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="6307a-111">[Enviar dados de diagnóstico para o seu espaço de trabalho](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="6307a-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="6307a-112">Você pode enviar dados de diagnóstico do seu locatário WVD para a Análise de Log do seu espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6307a-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="6307a-113">[Identificar e diagnosticar](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemas internos ou externos em relação à WVD.</span><span class="sxs-lookup"><span data-stu-id="6307a-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="6307a-114">Para saber mais sobre como configurar a ferramenta de diagnóstico de serviço para WVD, consulte Usar a Análise de Log para o recurso de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="6307a-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>
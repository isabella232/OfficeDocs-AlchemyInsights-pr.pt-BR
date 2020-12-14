---
title: Ferramenta de diagnóstico de serviço para área de trabalho virtual do Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665810"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="5d932-102">Ferramenta de diagnóstico de serviço para área de trabalho virtual do Windows</span><span class="sxs-lookup"><span data-stu-id="5d932-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="5d932-103">A área de trabalho virtual do Windows (WVD) oferece uma ferramenta de diagnóstico que permite que os administradores identifiquem erros através de uma única interface.</span><span class="sxs-lookup"><span data-stu-id="5d932-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="5d932-104">Esta ferramenta registra informações relacionadas a diagnóstico sempre que o WVD é usado por alguém que atribui uma função de WVD.</span><span class="sxs-lookup"><span data-stu-id="5d932-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="5d932-105">Cada log contém informações sobre a função WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e as informações sobre o locatário e o usuário.</span><span class="sxs-lookup"><span data-stu-id="5d932-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="5d932-106">A análise de logs do Azure pode ser configurada para capturar o log de atividades criado pela ferramenta de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="5d932-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="5d932-107">Veja como:</span><span class="sxs-lookup"><span data-stu-id="5d932-107">Here's how:</span></span>

1. <span data-ttu-id="5d932-108">Crie um espaço de trabalho da análise de logs com o [portal do Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="5d932-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="5d932-109">[Conectar computadores Windows ao Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="5d932-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="5d932-110">Obter a ID do espaço de trabalho e a chave primária do seu espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5d932-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="5d932-111">O assistente de instalação precisa dessas informações para configurar corretamente o agente e para garantir que ele possa se comunicar com o Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="5d932-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="5d932-112">[Enviar dados de diagnósticos por push para seu espaço de trabalho](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="5d932-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="5d932-113">Você pode enviar dados de diagnóstico do seu locatário do WVD para a análise de logs do seu espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5d932-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="5d932-114">[Identificar e diagnosticar problemas](https://go.microsoft.com/fwlink/?linkid=2128338) internos ou externos em relação ao WVD.</span><span class="sxs-lookup"><span data-stu-id="5d932-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="5d932-115">Para saber mais sobre como configurar a ferramenta de diagnóstico de serviço para o WVD, confira [usar a análise de logs para o recurso de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="5d932-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>

---
title: Corrigir remotamente problemas com a integração de dispositivos Windows 10 à Proteção Avançada contra Ameaças do Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735436"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="bc295-102">Corrigir remotamente problemas com a integração de dispositivos Windows 10 à Proteção Avançada contra Ameaças do Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="bc295-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="bc295-103">Se você puder acessar o computador remoto, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="bc295-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="bc295-104">Baixe a ferramenta de diagnóstico [Analisador de Conectividade do Cliente](https://go.microsoft.com/fwlink/?linkid=2143466).</span><span class="sxs-lookup"><span data-stu-id="bc295-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="bc295-105">Extraia e execute MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="bc295-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="bc295-106">Localize o log de diagnóstico na pasta MDATPClientAnalyzerResult, que é a mesma pasta onde a ferramenta Analisador foi baixada.</span><span class="sxs-lookup"><span data-stu-id="bc295-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="bc295-107">Para encontrar problemas com as configurações de conectividade ou proxy da Internet, revise o arquivo de log MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="bc295-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="bc295-108">Para saber mais, confira [Problemas com máquinas de integração.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="bc295-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>

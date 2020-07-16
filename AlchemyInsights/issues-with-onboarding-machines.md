---
title: Problemas com integração de computadores
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45138994"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="b08c0-102">Problemas com integração de computadores</span><span class="sxs-lookup"><span data-stu-id="b08c0-102">Issues with onboarding machines</span></span>

<span data-ttu-id="b08c0-103">Você pode ter problemas integrando os computadores com o serviço MDATP.</span><span class="sxs-lookup"><span data-stu-id="b08c0-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="b08c0-104">Se você puder acessar o computador do usuário final, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="b08c0-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="b08c0-105">Baixe a ferramenta de diagnóstico [Analisador de Conectividade do Cliente](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="b08c0-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="b08c0-106">Extraia e execute MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="b08c0-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="b08c0-107">Localize o log de diagnóstico na pasta chamada MDATPClientAnalyzerResult, a mesma pasta em que a ferramenta Analisador é baixada.</span><span class="sxs-lookup"><span data-stu-id="b08c0-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="b08c0-108">Examine o arquivo de log, MDATPClientAnalyzer.txt para encontrar problemas de conectividade ou configurações de proxy da internet.</span><span class="sxs-lookup"><span data-stu-id="b08c0-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>
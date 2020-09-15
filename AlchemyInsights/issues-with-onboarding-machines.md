---
title: Problemas com integração de computadores
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676870"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="26d2f-102">Problemas com integração de computadores</span><span class="sxs-lookup"><span data-stu-id="26d2f-102">Issues with onboarding machines</span></span>

<span data-ttu-id="26d2f-103">Você pode ter problemas integrando os computadores com o serviço MDATP.</span><span class="sxs-lookup"><span data-stu-id="26d2f-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="26d2f-104">Se você puder acessar o computador do usuário final, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="26d2f-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="26d2f-105">Baixe a ferramenta de diagnóstico [Analisador de Conectividade do Cliente](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="26d2f-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="26d2f-106">Extraia e execute MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="26d2f-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="26d2f-107">Localize o log de diagnóstico na pasta chamada MDATPClientAnalyzerResult, a mesma pasta em que a ferramenta Analisador é baixada.</span><span class="sxs-lookup"><span data-stu-id="26d2f-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="26d2f-108">Examine o arquivo de log, MDATPClientAnalyzer.txt para encontrar problemas de conectividade ou configurações de proxy da internet.</span><span class="sxs-lookup"><span data-stu-id="26d2f-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>
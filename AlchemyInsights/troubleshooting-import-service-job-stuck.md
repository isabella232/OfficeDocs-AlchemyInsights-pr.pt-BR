---
title: Trabalho de Solução de Problemas do Serviço de Importação Travado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059838"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="ad0d3-102">Trabalho de Solução de Problemas do Serviço de Importação Travado</span><span class="sxs-lookup"><span data-stu-id="ad0d3-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="ad0d3-103">Se você estiver tendo problemas com os trabalhos do serviço de Importação travados ou com falha, examine e tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ad0d3-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="ad0d3-104">Analise o tamanho do arquivo PST.</span><span class="sxs-lookup"><span data-stu-id="ad0d3-104">Review the size of of the PST file.</span></span> <span data-ttu-id="ad0d3-105">O tamanho máximo recomendado de um arquivo PST para importação é 20 GB.</span><span class="sxs-lookup"><span data-stu-id="ad0d3-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="ad0d3-106">Se você suspeitar de itens ignorados devido à corrupção, execute Scanpst.exe para diagnosticar e corrigir erros nos arquivos PST.</span><span class="sxs-lookup"><span data-stu-id="ad0d3-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="ad0d3-107">Se você vir um erro "MapiExceptionShutoffQuotaExceeded" durante a importação, certifique-se de que a caixa de correio de destino tenha capacidade suficiente para importar os arquivos PST desejados.</span><span class="sxs-lookup"><span data-stu-id="ad0d3-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="ad0d3-108">Para obter mais informações sobre como solucionar Problemas de trabalho de importação PST, confira [Solucionar problemas com trabalhos de importação PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="ad0d3-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="ad0d3-109">Para obter informações sobre como corrigir problemas ao importar PST para o Outlook, confira [Corrigir problemas ao importar um arquivo .pst do Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="ad0d3-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>
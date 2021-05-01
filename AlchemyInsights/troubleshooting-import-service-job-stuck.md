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
# <a name="troubleshooting-import-service-job-stuck"></a>Trabalho de Solução de Problemas do Serviço de Importação Travado

Se você estiver tendo problemas com os trabalhos do serviço de Importação travados ou com falha, examine e tente o seguinte:

- Analise o tamanho do arquivo PST. O tamanho máximo recomendado de um arquivo PST para importação é 20 GB.

- Se você suspeitar de itens ignorados devido à corrupção, execute Scanpst.exe para diagnosticar e corrigir erros nos arquivos PST.

- Se você vir um erro "MapiExceptionShutoffQuotaExceeded" durante a importação, certifique-se de que a caixa de correio de destino tenha capacidade suficiente para importar os arquivos PST desejados.

Para obter mais informações sobre como solucionar Problemas de trabalho de importação PST, confira [Solucionar problemas com trabalhos de importação PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Para obter informações sobre como corrigir problemas ao importar PST para o Outlook, confira [Corrigir problemas ao importar um arquivo .pst do Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).
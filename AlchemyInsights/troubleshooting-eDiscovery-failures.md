---
title: 1490-Troubleshooting-eDiscovery-Failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277819"
---
# <a name="troubleshoot-content-search-errors"></a>Solucionar erros de pesquisa de conteúdo

Você está tendo problemas com a pesquisa de conteúdo ou obtendo falhas ao exportar resultados de pesquisa?

Por exemplo, você recebe o seguinte ao executar pesquisas?

- Erros CS008 ou CS012

- Erros de tempo limite do servidor

- Ocorreu um erro de aplicativo

Ou ao pesquisar ou exportar resultados de um grande número de caixas de correio (mais de 100.000 caixas de correio), você está recebendo erros de exportação?

Para esses tipos de erros, tente pesquisar os locais de conteúdo que falharam. Confira  [Este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obter mais informações.

Se você estiver exportando mais de 100.000 caixas de correio, será necessário usar o seguinte PowerShell para baixar os resultados da exportação:  [exportação de resultados de mais de 100.000 caixas de correio](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).

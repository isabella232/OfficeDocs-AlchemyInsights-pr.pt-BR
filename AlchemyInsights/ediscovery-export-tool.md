---
title: Ferramenta de exportação de Descoberta Eletrônica
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101290"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Não é possível instalar ou executar a Ferramenta de Exportação de Descoberta Digital?

Se você não puder instalar ou executar a Ferramenta de Exportação de Descoberta Digital para baixar os resultados da pesquisa, verifique as seguintes coisas:
  
- O computador que você está usando atende a esses pré-requisitos:

  - Versões de 32 e 64 bits do Windows 7 e versões posteriores

  - Microsoft .NET Framework 4.7

  - Um navegador com suporte:

  - Microsoft Edge

    Ou

  - Internet Explorer 10 e versões posteriores

    Não há suporte para outros navegadores, como o Google Chrome e o Mozilla Firefox.

- Sua organização pode se conectar ao ponto de extremidade no Azure, que é **\* .blob.core.windows.net** (o curinga representa um identificador exclusivo para seu trabalho de exportação).

- Você recebe a função Exportar no Centro de Conformidade Microsoft 365 &amp; Segurança. Por padrão, essa função é atribuída apenas ao grupo de funções do Gerenciador de Descobertas. Consulte [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Para obter mais informações, consulte [Exportar resultados da Pesquisa de Conteúdo](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Se você estiver exportando mais de 100.000 caixas de correio, você precisará usar o Powershell a seguir para baixar os resultados de Exportação: Exportando resultados de mais de  [100.000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)caixas de correio .
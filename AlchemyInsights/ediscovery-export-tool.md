---
title: Ferramenta de exportação de Descoberta Eletrônica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36736313"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Não é possível instalar ou executar a ferramenta de exportação de descoberta eletrônica?

Se você não conseguir instalar ou executar a ferramenta de exportação de descoberta eletrônica do Office 365 para baixar os resultados da pesquisa, verifique as seguintes coisas:
  
- O computador que você está usando atende a esses pré-requisitos:

  - Versões de 32 e 64 bits do Windows 7 e versões posteriores

  - Microsoft .NET Framework 4,7

  - Um navegador com suporte:

  - Microsoft Edge

    Ou

  - Internet Explorer 10 e versões posteriores

    Outros navegadores, como Google Chrome e Mozilla Firefox, não são suportados.

- Sua organização pode se conectar ao ponto de extremidade no Azure, que é ** \*. blob.Core.Windows.net** (o caractere curinga representa um identificador exclusivo para seu trabalho de exportação).

- Você é atribuído à função exportar no centro de conformidade de &amp; segurança do Office 365. Por padrão, essa função só é atribuída ao grupo de função Gerenciador de descoberta eletrônica. Consulte [atribuir permissões de descoberta eletrônica](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Para obter mais informações, consulte [Exportar resultados de pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  
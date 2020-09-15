---
title: Ferramenta de exportação de Descoberta Eletrônica
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711083"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Não é possível instalar ou executar a ferramenta de exportação de descoberta eletrônica?

Se você não conseguir instalar ou executar a ferramenta de exportação de descoberta eletrônica para baixar os resultados da pesquisa, verifique as seguintes coisas:
  
- O computador que você está usando atende a esses pré-requisitos:

  - Versões de 32 e 64 bits do Windows 7 e versões posteriores

  - Microsoft .NET Framework 4.7

  - Um navegador com suporte:

  - Microsoft Edge

    Ou

  - Internet Explorer 10 e versões posteriores

    Outros navegadores, como Google Chrome e Mozilla Firefox, não são suportados.

- Sua organização pode se conectar ao ponto de extremidade no Azure, que é ** \* . blob.Core.Windows.net** (o caractere curinga representa um identificador exclusivo para seu trabalho de exportação).

- Você é atribuído à função exportar no centro de conformidade de segurança do Microsoft 365 &amp; . Por padrão, essa função só é atribuída ao grupo de função Gerenciador de descoberta eletrônica. Consulte [atribuir permissões de descoberta eletrônica](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Para obter mais informações, consulte [Exportar resultados de pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  
---
title: Não sincronização do Active Directory
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822839"
---
# <a name="active-directory-not-syncing"></a>Não sincronização do Active Directory

Se você estiver recebendo erros de sincronização, como "nenhuma sincronização recente", ou observe que o status de sincronização de diretório no portal de administração do Office diz: "A última sincronização foi há mais de 3 dias", pode ser que o AADConnect tenha configurações incorretas ou permissões insuficientes para executar uma sincronização.  

Reinstalar o AADConnect usando configurações expressas pode resolver o problema rapidamente:

1. [Baixe a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga as instruções para instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Para mais informações sobre contas de serviço do AADConnect, confira [Azure AD Connect: Contas e permissões](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).

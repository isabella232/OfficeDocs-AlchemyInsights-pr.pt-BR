---
title: O Active Directory não está sincronizando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265121"
---
# <a name="active-directory-not-syncing"></a>O Active Directory não está sincronizando

Se você estiver recebendo erros de sincronização, como "nenhuma sincronização recente" ou Observe que o status de sincronização do diretório no portal de administração do Office diz, "última sincronização há mais de três dias", pode ser que o AADConnect tenha configurações incorretas ou insuficientes permissões para executar uma sincronização.  

A reinstalação do AADConnect usando as configurações expressas pode resolver o problema rapidamente:

1. [Baixe a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga as instruções para a instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Para obter mais informações sobre contas de serviço do AADConnect, consulte [Azure ad Connect: Accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).

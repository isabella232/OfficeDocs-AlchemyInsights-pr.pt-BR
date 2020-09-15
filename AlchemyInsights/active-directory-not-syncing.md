---
title: O Active Directory não está sincronizando
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697617"
---
# <a name="active-directory-not-syncing"></a>O Active Directory não está sincronizando

Se você estiver recebendo erros de sincronização, como "sem sincronização recente", ou Observe que o status de sincronização do diretório no portal de administração do Office diz, "última sincronização há mais de três dias", pode ser que o AADConnect tenha configurações incorretas ou permissões insuficientes para executar uma sincronização.  

A reinstalação do AADConnect usando as configurações expressas pode resolver o problema rapidamente:

1. [Baixe a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga as instruções para a instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Para mais informações sobre contas de serviço do AADConnect, confira [Azure AD Connect: Contas e permissões](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).

---
title: Pasta pública habilitada para enviar como email no EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394684"
---
# <a name="sendas-mail-enabled-public-folder"></a>Pasta pública de sendas habilitada para email

O exemplo a seguir atribui permissões "Send as" para a pasta pública habilitada para email NewPF1 para o usuário Jason.

Add-RecipientPermission-Identity ' NewPF1 '-trustee "Jason"-AccessRights ' sendas '

Para informações detalhadas de sintaxes e de parâmetros, consulte [atribuir permissões "enviar como" ou "enviar em nome" para pastas públicas habilitadas para email](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

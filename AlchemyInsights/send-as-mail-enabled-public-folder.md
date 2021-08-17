---
title: Enviar como pasta pública habilitada para email no EXO
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
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052554"
---
# <a name="sendas-mail-enabled-public-folder"></a>Pasta pública habilitada para Email SendAs

O exemplo a seguir atribui permissões "Enviar como" para a pasta pública habilitada para email NewPF1 ao usuário Jasão.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jasão" -AccessRights 'SendAs'

Para obter informações detalhadas sobre sintaxes e [parâmetros, consulte Atribuir permissões "Enviar como"](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)ou "Enviar em nome" para pastas públicas habilitadas para email.


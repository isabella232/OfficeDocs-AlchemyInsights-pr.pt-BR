---
title: Código de erro 550 5.7.501 acesso negado, abuso de spam detectado
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784043"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 acesso negado, abuso de spam detectado

Normalmente, essa mensagem ocorre quando os usuários enviam mensagens de email de endereços IP usando o domínio inicial *. onmicrosoft.com* atribuído aos novos locatários no Microsoft 365. A maneira mais fácil de resolver esse problema é:

1. [Adicionar um domínio ao seu locatário](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Altere o endereço de email principal do usuário](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) para o novo domínio personalizado que você acabou de adicionar.

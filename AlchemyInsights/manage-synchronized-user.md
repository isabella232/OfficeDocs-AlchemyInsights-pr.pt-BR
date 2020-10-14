---
title: Gerenciar usuário sincronizado
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451388"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Não é possível definir o endereço de email principal, alterar os atributos do usuário ou remover/excluir um usuário sincronizado

Se a sincronização de diretórios estiver habilitada para seu ambiente, alguns atributos de usuário ou de objeto não poderão ser alterados usando o centro de administração do Microsoft 365.

Para gerenciar totalmente os usuários sincronizados e todos os seus atributos, use o console de gerenciamento de usuários e grupos do Active Directory local (Adsiedit. msc).  

Como alternativa, você pode alterar usuários ou atributos individuais para usuários sincronizados usando o PowerShell, como mostrado nesses exemplos comuns:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`

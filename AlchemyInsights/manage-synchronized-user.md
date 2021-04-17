---
title: Gerenciar Usuário Sincronizado
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823955"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Não é possível definir o endereço de email principal, alterar atributos do usuário ou remover/excluir um usuário sincronizado

Se a sincronização de diretório estiver habilitada para seu ambiente, alguns atributos de usuário ou objeto não poderão ser alterados usando o Centro de administração do Microsoft 365.

Para gerenciar totalmente usuários sincronizados e todos os atributos, use o console de gerenciamento de grupos e usuários do active directory local (adsiedit.msc).  

Como alternativa, você pode alterar usuários individuais ou atributos para usuários sincronizados usando o powershell, como mostrado nestes exemplos comuns:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`

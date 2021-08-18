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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114749"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Não é possível definir o endereço de email principal, alterar atributos do usuário ou remover/excluir um usuário sincronizado

Se a sincronização de diretório estiver habilitada para seu ambiente, alguns atributos de usuário ou objeto não poderão ser alterados usando a Centro de administração do Microsoft 365.

Para gerenciar totalmente usuários sincronizados e todos os atributos, use o console de gerenciamento de grupos e usuários do active directory local (adsiedit.msc).  

Como alternativa, você pode alterar usuários individuais ou atributos para usuários sincronizados usando o powershell, como mostrado nestes exemplos comuns:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`

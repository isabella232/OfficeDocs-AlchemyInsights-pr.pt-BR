---
title: Problemas com o MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098590"
---
# <a name="issues-with-azure-mfa"></a>Problemas com o Azure MFA
Há algumas coisas para verificar se os usuários não podem fazer logoff usando a autenticação multifafatória (MFA)

1. O usuário afetado pode ser bloqueado no portal Azure Active Directory Portal. Se esse for o caso, as tentativas de autenticação para esse usuário específico serão negadas automaticamente. [Siga as etapas deste artigo para desbloqueá-las.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se o desbloqueio do usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir o MFA para o usuário e ele passará pelo processo de registro novamente. [Siga as etapas deste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se essa for a primeira vez que você habilitar o MFA e os usuários não puderem fazer logon em clientes que não sejam navegadores, como Outlook, Skype, etc, talvez o ADAL (Biblioteca de Autenticação do Active Directory) não esteja habilitado na sua assinatura do O365. Nesse caso, você precisará se conectar ao Exchange Online Powershell e executar este cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*
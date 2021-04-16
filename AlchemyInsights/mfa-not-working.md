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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810472"
---
# <a name="issues-with-azure-mfa"></a>Problemas com o Azure MFA
Há algumas coisas para verificar se os usuários não podem fazer logoff usando a autenticação multifafatória (MFA)

1. O usuário afetado pode ser bloqueado no Portal do Azure Active Directory. Se esse for o caso, as tentativas de autenticação para esse usuário específico serão negadas automaticamente. [Siga as etapas deste artigo para desbloqueá-las.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se o desbloqueio do usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir o MFA para o usuário e ele passará pelo processo de registro novamente. [Siga as etapas deste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se essa for a primeira vez que você habilitar o MFA e seus usuários não puderem fazer logon em clientes que não sejam navegadores, como Outlook, Skype, etc., talvez a ADAL (Biblioteca de Autenticação do Active Directory) não esteja habilitada em sua assinatura do O365. Nesse caso, você precisará se conectar ao Powershell do Exchange Online e executar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*
---
title: Problemas com a MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768825"
---
# <a name="issues-with-azure-mfa"></a>Problemas com o Azure MFA
Há algumas coisas para verificar se os usuários não podem fazer logon usando a autenticação multifator (MFA)

1. O usuário afetado pode ser bloqueado no portal do Azure Active Directory. Se esse for o caso, as tentativas de autenticação desse usuário específico serão automaticamente negadas. [Siga as etapas deste artigo para desbloqueá-los.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se o usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir o MFA para o usuário e ele passará pelo processo de inscrição novamente. [Siga as etapas neste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se esta é a primeira vez que você habilitou o MFA e seus usuários não conseguem fazer logon em clientes que não são do navegador, como Outlook, Skype, etc., talvez ADAL (biblioteca de autenticação do Active Directory) não está habilitado em sua assinatura do O365. Nesse caso, você precisará se conectar ao PowerShell do Exchange Online e executar este cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*
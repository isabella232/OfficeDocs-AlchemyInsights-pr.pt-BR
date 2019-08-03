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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250153"
---
# <a name="issues-with-mfa"></a>Problemas com a MFA
Há algumas coisas para verificar se os usuários não podem fazer logon usando a autenticação multifator (MFA)

1. O usuário afetado pode ser bloqueado no portal do Azure Active Directory. Se esse for o caso, as tentativas de autenticação desse usuário específico serão automaticamente negadas. [Siga as etapas deste artigo para desbloqueá-los.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se o usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir o MFA para o usuário e ele passará pelo processo de inscrição novamente. [Siga as etapas neste artigo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se esta é a primeira vez que você habilitou o MFA e seus usuários não conseguem fazer logon em clientes que não são do navegador, como Outlook, Skype, etc., talvez ADAL (biblioteca de autenticação do Active Directory) não está habilitado em sua assinatura do O365. Nesse caso, você precisará se conectar ao PowerShell do Exchange Online e executar este cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*
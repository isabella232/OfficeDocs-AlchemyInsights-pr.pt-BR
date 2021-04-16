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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="33b83-102">Problemas com o Azure MFA</span><span class="sxs-lookup"><span data-stu-id="33b83-102">Issues with Azure MFA</span></span>
<span data-ttu-id="33b83-103">Há algumas coisas para verificar se os usuários não podem fazer logoff usando a autenticação multifafatória (MFA)</span><span class="sxs-lookup"><span data-stu-id="33b83-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="33b83-104">O usuário afetado pode ser bloqueado no Portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="33b83-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="33b83-105">Se esse for o caso, as tentativas de autenticação para esse usuário específico serão negadas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33b83-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="33b83-106">Siga as etapas deste artigo para desbloqueá-las.</span><span class="sxs-lookup"><span data-stu-id="33b83-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="33b83-107">Se o desbloqueio do usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir o MFA para o usuário e ele passará pelo processo de registro novamente.</span><span class="sxs-lookup"><span data-stu-id="33b83-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="33b83-108">Siga as etapas deste artigo.</span><span class="sxs-lookup"><span data-stu-id="33b83-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="33b83-109">Se essa for a primeira vez que você habilitar o MFA e seus usuários não puderem fazer logon em clientes que não sejam navegadores, como Outlook, Skype, etc., talvez a ADAL (Biblioteca de Autenticação do Active Directory) não esteja habilitada em sua assinatura do O365.</span><span class="sxs-lookup"><span data-stu-id="33b83-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="33b83-110">Nesse caso, você precisará se conectar ao Powershell do Exchange Online e executar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="33b83-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
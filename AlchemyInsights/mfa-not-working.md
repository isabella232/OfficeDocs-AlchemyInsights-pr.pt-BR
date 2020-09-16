---
title: Problemas com a MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755119"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="a3587-102">Problemas com o Azure MFA</span><span class="sxs-lookup"><span data-stu-id="a3587-102">Issues with Azure MFA</span></span>
<span data-ttu-id="a3587-103">Há algumas coisas para verificar se os usuários não podem fazer logon usando a autenticação multifator (MFA)</span><span class="sxs-lookup"><span data-stu-id="a3587-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="a3587-104">O usuário afetado pode ser bloqueado no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a3587-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="a3587-105">Se esse for o caso, as tentativas de autenticação desse usuário específico serão automaticamente negadas.</span><span class="sxs-lookup"><span data-stu-id="a3587-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="a3587-106">Siga as etapas deste artigo para desbloqueá-los.</span><span class="sxs-lookup"><span data-stu-id="a3587-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="a3587-107">Se o usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir o MFA para o usuário e ele passará pelo processo de inscrição novamente.</span><span class="sxs-lookup"><span data-stu-id="a3587-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="a3587-108">Siga as etapas neste artigo.</span><span class="sxs-lookup"><span data-stu-id="a3587-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="a3587-109">Se esta é a primeira vez que você habilitou o MFA e seus usuários não conseguem fazer logon em clientes que não são do navegador, como Outlook, Skype, etc., talvez ADAL (biblioteca de autenticação do Active Directory) não está habilitado em sua assinatura do O365.</span><span class="sxs-lookup"><span data-stu-id="a3587-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="a3587-110">Nesse caso, você precisará se conectar ao PowerShell do Exchange Online e executar este cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="a3587-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
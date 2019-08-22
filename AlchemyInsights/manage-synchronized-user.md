---
title: Gerenciar usuário sincronizado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541969"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="0a7aa-102">Não é possível definir o endereço de email principal ou alterar os atributos do usuário</span><span class="sxs-lookup"><span data-stu-id="0a7aa-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="0a7aa-103">Se a sincronização de diretórios estiver habilitada para seu ambiente, alguns atributos de usuário ou de objeto não poderão ser alterados usando o centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0a7aa-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="0a7aa-104">Para gerenciar totalmente os usuários sincronizados e todos os seus atributos, use o console de gerenciamento de usuários e grupos do Active Directory local (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="0a7aa-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="0a7aa-105">Como alternativa, você pode alterar usuários ou atributos individuais para usuários sincronizados usando o PowerShell, como mostrado nesses exemplos comuns:</span><span class="sxs-lookup"><span data-stu-id="0a7aa-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="0a7aa-106">Set-MsolUser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="0a7aa-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="0a7aa-107">Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "user"-title "Manager"-Department "HR" h</span><span class="sxs-lookup"><span data-stu-id="0a7aa-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="0a7aa-108">Remove-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="0a7aa-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>
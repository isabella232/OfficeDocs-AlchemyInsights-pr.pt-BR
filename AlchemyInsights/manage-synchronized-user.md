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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="3c221-102">Não é possível definir o endereço de email principal, alterar atributos do usuário ou remover/excluir um usuário sincronizado</span><span class="sxs-lookup"><span data-stu-id="3c221-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="3c221-103">Se a sincronização de diretório estiver habilitada para seu ambiente, alguns atributos de usuário ou objeto não poderão ser alterados usando o Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3c221-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="3c221-104">Para gerenciar totalmente usuários sincronizados e todos os atributos, use o console de gerenciamento de grupos e usuários do active directory local (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="3c221-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="3c221-105">Como alternativa, você pode alterar usuários individuais ou atributos para usuários sincronizados usando o powershell, como mostrado nestes exemplos comuns:</span><span class="sxs-lookup"><span data-stu-id="3c221-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`

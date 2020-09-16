---
title: O usuário único não está vendo suplementos no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719653"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="3f958-102">O usuário único não está vendo suplementos no Outlook</span><span class="sxs-lookup"><span data-stu-id="3f958-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="3f958-103">O usuário pode fazer parte de uma função que não tem o parâmetro AppsForOfficeEnabled correto.</span><span class="sxs-lookup"><span data-stu-id="3f958-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="3f958-104">Execute esse cmdlet para descobrir se a função correta está associada ao usuário:</span><span class="sxs-lookup"><span data-stu-id="3f958-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="3f958-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="3f958-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="3f958-106">Para obter mais informações, consulte [Especificar os administradores e usuários que podem instalar e gerenciar suplementos do Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="3f958-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

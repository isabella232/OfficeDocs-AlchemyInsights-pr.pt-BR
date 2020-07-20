---
title: O usuário único não está vendo suplementos no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154542"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>O usuário único não está vendo suplementos no Outlook

O usuário pode fazer parte de uma função que não tem o parâmetro AppsForOfficeEnabled correto. Execute esse cmdlet para descobrir se a função correta está associada ao usuário:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Para obter mais informações, consulte [Especificar os administradores e usuários que podem instalar e gerenciar suplementos do Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

---
title: Diversos usuários recebem o erro Acesso Negado ao adicionar suplementos ao Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724351"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="98381-102">Diversos usuários recebem o erro Acesso Negado ao adicionar suplementos ao Outlook</span><span class="sxs-lookup"><span data-stu-id="98381-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="98381-103">Você pode especificar quais administradores na sua organização têm permissão para instalar e gerenciar suplementos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="98381-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="98381-104">Você pode também especificar quais administradores na sua organização têm permissão para instalar e gerenciar suplementos para seu próprio uso.</span><span class="sxs-lookup"><span data-stu-id="98381-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="98381-105">Para obter mais detalhes, confira o artigo [Especificar os administradores e usuários que podem instalar e gerenciar suplementos do Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="98381-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="98381-106">Para verificar se você conseguiu atribuir permissões a um usuário, substitua <Role Name> pelo nome da função a ser verificada e execute o seguinte comando no PowerShell do Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="98381-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="98381-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="98381-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="98381-108">Esse exemplo mostra como verificar para quem você atribuiu permissões para instalar suplementos da Office Store na organização.</span><span class="sxs-lookup"><span data-stu-id="98381-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="98381-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="98381-109">PowerShell</span></span>

<span data-ttu-id="98381-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="98381-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="98381-111">Nos resultados, Get-ManagementRoleAssignment, verifique as entradas na coluna Usuários Efetivos.</span><span class="sxs-lookup"><span data-stu-id="98381-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="98381-112">Para informações detalhadas de sintaxes e de parâmetros, consulte [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="98381-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 
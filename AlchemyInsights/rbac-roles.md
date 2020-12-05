---
title: 'Funções RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576350"
---
# <a name="rbac-rules"></a><span data-ttu-id="0c7bb-102">Regras RBAC</span><span class="sxs-lookup"><span data-stu-id="0c7bb-102">RBAC rules</span></span>

<span data-ttu-id="0c7bb-103">Se você receber o erro de permissão:</span><span class="sxs-lookup"><span data-stu-id="0c7bb-103">If you get the permission error:</span></span> 

- <span data-ttu-id="0c7bb-104">**O cliente com ID de objeto não tem autorização para executar a ação sobre escopo (código: AuthorizationFailed)**: ao tentar criar um recurso, verifique se você está conectado atualmente com um usuário que tenha uma função que tenha permissão de gravação para o recurso no escopo selecionado.</span><span class="sxs-lookup"><span data-stu-id="0c7bb-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="0c7bb-105">Por exemplo, para gerenciar máquinas virtuais em um grupo de recursos, você deve ter a função de [colaborador da máquina virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) no grupo de recursos (ou escopo pai).</span><span class="sxs-lookup"><span data-stu-id="0c7bb-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="0c7bb-106">Para obter uma lista das permissões para cada função interna, consulte [funções internas para recursos do Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0c7bb-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="0c7bb-107">**Você não tem permissão para criar uma solicitação de suporte**: ao tentar criar ou atualizar um tíquete de suporte, verifique se você está conectado atualmente com um usuário que é atribuído a uma função que tenha a permissão Microsoft. support/supportTickets/Write, como o [colaborador de solicitação de suporte](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="0c7bb-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="0c7bb-108">**Nenhuma atribuição de função pode ser criada (código: RoleAssignmentLimitExceeded)**: ao tentar atribuir uma função, tente reduzir o número de atribuições de função, atribuindo funções a grupos.</span><span class="sxs-lookup"><span data-stu-id="0c7bb-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="0c7bb-109">O Azure oferece suporte a até **2000** atribuições de função por assinatura.</span><span class="sxs-lookup"><span data-stu-id="0c7bb-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="0c7bb-110">Para obter mais detalhes sobre as funções do Azure RBAC, consulte [funções do Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0c7bb-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

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
# <a name="rbac-rules"></a>Regras RBAC

Se você receber o erro de permissão: 

- **O cliente com ID de objeto não tem autorização para executar a ação sobre escopo (código: AuthorizationFailed)**: ao tentar criar um recurso, verifique se você está conectado atualmente com um usuário que tenha uma função que tenha permissão de gravação para o recurso no escopo selecionado. Por exemplo, para gerenciar máquinas virtuais em um grupo de recursos, você deve ter a função de [colaborador da máquina virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) no grupo de recursos (ou escopo pai). Para obter uma lista das permissões para cada função interna, consulte [funções internas para recursos do Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Você não tem permissão para criar uma solicitação de suporte**: ao tentar criar ou atualizar um tíquete de suporte, verifique se você está conectado atualmente com um usuário que é atribuído a uma função que tenha a permissão Microsoft. support/supportTickets/Write, como o [colaborador de solicitação de suporte](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Nenhuma atribuição de função pode ser criada (código: RoleAssignmentLimitExceeded)**: ao tentar atribuir uma função, tente reduzir o número de atribuições de função, atribuindo funções a grupos. O Azure oferece suporte a até **2000** atribuições de função por assinatura.

Para obter mais detalhes sobre as funções do Azure RBAC, consulte [funções do Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

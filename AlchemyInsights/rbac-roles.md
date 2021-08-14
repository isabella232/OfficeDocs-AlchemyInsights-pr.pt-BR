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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923113"
---
# <a name="rbac-rules"></a>Regras do RBAC

Se você receber o erro de permissão: 

- O cliente com a ID do objeto não tem autorização para executar a ação sobre o escopo **(código: AuthorizationFailed)**: ao tentar criar um recurso, verifique se você está atualmente se inscreveu com um usuário que recebe uma função que tem permissão de gravação para o recurso no escopo selecionado. Por exemplo, para gerenciar máquinas virtuais em um grupo de recursos, você deve ter a função Colaborador da Máquina [Virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) no grupo de recursos (ou escopo pai). Para ver uma lista das permissões para cada função in-loco, consulte [Funções embutidas para recursos do Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Você não tem permissão para criar uma solicitação de **suporte:** ao tentar criar ou atualizar um tíquete de suporte, verifique se você está atualmente se inscreveu com um usuário que recebe uma função que tem a permissão Microsoft.Support/supportTickets/write, como [Colaborador](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)de Solicitação de Suporte.
- Não é possível criar mais atribuições de função **(código: RoleAssignmentLimitExceeded)**: ao tentar atribuir uma função, tente reduzir o número de atribuições de função atribuindo funções a grupos. O Azure dá suporte a até **2.000 atribuições** de função por assinatura.

Para obter mais detalhes sobre funções do Azure RBAC, consulte [Funções do Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

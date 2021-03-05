---
title: Problema com um único usuário
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428505"
---
# <a name="problem-with-single-user"></a>Problema com um único usuário

- O usuário pode não ter sido provisionado porque o serviço ainda não teve a chance de avaliar o usuário. Revise as diretrizes de quanto tempo o provisionamento leva, bem como a barra de progresso na página de configuração de provisionamento. Se o estado estável especificado na seção de detalhes adicionais for antes da data em que o usuário foi criado/atualizado/excluído, isso significa que ainda não avaliamos o usuário. Nesse cenário, o melhor a fazer é aguardar o fim do serviço de provisionamento.

  - Observe que nosso serviço só está ciente das alterações em um usuário no sistema de origem (Cloud HR). Deve haver uma alteração válida no sistema de origem do Azure AD para detectar a alteração e fluí-la para o Active Directory.
- O serviço de provisionamento avaliou o usuário e determinou que ele não deve ser provisionado:
  - Se você tiver definido um filtro de scoping baseado em atributo, verifique se o usuário atende aos critérios especificados.
  - Se os usuários já existirem no sistema de destino e no estado do usuário na origem e na combinação de destino, não tomaremos mais nenhuma ação.
- O serviço de provisionamento tentou provisionar o usuário e falhou. Para esses cenários, revise a guia solução de problemas e recomendações dos logs de provisionamento:
  - Um atributo necessário no usuário pode estar ausente no Active Directory local ou no Azure AD. Por exemplo, as regras de geração userPrincipalName ou sAMAccountName não estão gerando o valor certo.
  - O atributo matching (geralmente employeeId) não está sendo resolvido para um usuário exclusivo no Active Directory local ou no Azure AD. Por exemplo, há dois usuários com o mesmo employeeId no AD e o serviço retorna um código de erro indicando entradas de destino duplicadas para a mesma entrada de origem.

Para revisar logs para um único usuário e grupos, consulte [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).

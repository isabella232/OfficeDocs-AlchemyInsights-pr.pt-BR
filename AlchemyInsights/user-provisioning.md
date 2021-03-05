---
title: Provisionamento de usuário
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430709"
---
# <a name="user-provisioning"></a>Provisionamento de usuário

- Use o [recurso de provisionamento](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) sob demanda para provisionar um usuário e obter diagnósticos detalhados sobre as etapas realizadas.
- Para solucionar problemas encontrados durante o provisionamento de usuários e grupos, consulte o guia de solução de problemas [Nenhum usuário está sendo provisionado para](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Se você observar que os usuários não estão sendo provisionados, consulte [Logs de provisionamento (visualização)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) no Azure Active Directory (AD). Procure entradas de log referentes a um usuário específico.
- Reinicie periodicamente o provisionamento para capturar todos os usuários que não foram encontrados em um ciclo de provisionamento anterior.
- O usuário/grupo pode não ter sido provisionado porque nosso serviço ainda não teve a chance de avaliar o usuário. Revise as diretrizes de quanto tempo o provisionamento leva, bem como a barra de progresso na página de configuração de provisionamento. Se o estado estável especificado na seção de detalhes adicionais for antes da data em que o usuário foi criado/atualizado/excluído, isso significa que ainda não avaliamos o usuário. Nesse cenário, o melhor a fazer é aguardar o fim do serviço de provisionamento. Se o estado estável tiver sido atingido, recomendamos executar uma reinicialização da interface do usuário no Portal do Azure.
  - Observe que nosso serviço só está ciente das alterações em um usuário/grupo no sistema de origem (Azure Active Directory). Se um usuário/grupo for removido diretamente no aplicativo (por exemplo, ServiceNow), não estamos cientes dessas alterações e não o reverteremos com base no estado do usuário no sistema de origem. Nesse cenário, é melhor reverter a alteração diretamente no aplicativo de destino.
- Nosso serviço avaliou o usuário/grupo e determinou que ele não deve ser provisionado:
  - Se você definiu o escopo como usuários e grupos atribuídos, verifique se o usuário/grupo está atribuído ao aplicativo.
  - Se o usuário/grupo for atribuído ao aplicativo, verifique se ele não está atribuído à função de acesso padrão. Essa função não pode ser usada para provisionamento.
  - Se você tiver definido um filtro de scoping baseado em atributo, verifique se o usuário atende aos critérios especificados.
  - Se os usuários já existirem no sistema de destino e no estado do usuário na origem e na combinação de destino, não tomaremos mais nenhuma ação.
- Nosso serviço tentou provisionar o usuário e falhou. Para esses cenários, revise a guia solução de problemas e recomendações dos logs de provisionamento:
  - Um atributo necessário no usuário pode estar ausente no Azure Active Directory ou não corresponder ao formato exigido pelo aplicativo de terceiros. Por exemplo, o atributo Country em um usuário pode ser definido como Estados Unidos quando deve ser EUA.
  - O atributo é um atributo referencial que ainda não existe no aplicativo de destino. Um atributo referencial é um atributo que aponta para outro objeto, por exemplo, um usuário que é membro de um grupo. A ID do usuário estaria no atributo membro do grupo, mas só poderá ser processada se o objeto do usuário que ele aponta já existir.

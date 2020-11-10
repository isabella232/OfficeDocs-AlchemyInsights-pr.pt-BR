---
title: Comentários sobre itens de lista
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947472"
---
# <a name="comments-on-list-items"></a>Comentários sobre itens de lista

Em breve, os usuários poderão adicionar e excluir comentários em itens de lista. Os usuários podem exibir todos os comentários em um item de lista e filtrar entre modos de exibição que mostram comentários ou atividades relacionadas a um item.

**Tempo** :

**Lançamento direcionado** : distribuição gradual em meados de outubro e esperado para conclusão em meados de novembro

**Versão padrão** : distribuição gradual em meados de novembro e espera-se que seja concluída pelo início de dezembro

**Distribuição** : lançamento direcionado para toda a organização

Os usuários precisam observar o seguinte antes de poderem adicionar e excluir comentários:

- Os comentários seguem as configurações de permissão inerentes no SharePoint.
- Listas clássicas que ainda não foram criadas para exibição em interfaces de usuário modernas, como listas de tarefas, não terão este recurso de comentários.
- O comentário em listas no Microsoft Teams não está disponível nesta versão.
- Os comentários não são indexados pela pesquisa.

Os administradores podem desabilitar esse recurso no nível da organização alterando o parâmetro **CommentsOnListItemsDisabled** no cmdlet do PowerShell **set-SPOTenant** .

No momento, não é possível desabilitar o comentário no nível do site ou da lista. Esperamos ter esses controles em uma atualização posterior, provavelmente no primeiro trimestre de 2021.

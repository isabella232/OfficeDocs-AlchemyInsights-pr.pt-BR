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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724142"
---
# <a name="comments-on-list-items"></a>Comentários sobre itens de lista

Os usuários podem exibir todos os comentários em um item de lista e filtrar entre modos de exibição que mostram comentários ou atividades relacionadas a um item.

Os usuários precisam observar o seguinte antes de poderem adicionar e excluir comentários:

- Os comentários seguem as configurações de permissão inerentes no SharePoint.
- Listas clássicas que ainda não foram criadas para exibição em interfaces de usuário modernas, como listas de tarefas, não terão este recurso de comentários.
- O comentário em listas no Microsoft Teams não está disponível nesta versão.
- Os comentários não são indexados pela pesquisa.

Os administradores podem desabilitar esse recurso no nível da organização alterando o parâmetro **CommentsOnListItemsDisabled** no cmdlet do PowerShell **set-SPOTenant** .

No momento, não é possível desabilitar o comentário no nível do site ou da lista. Esperamos ter esses controles em uma atualização posterior, provavelmente no primeiro trimestre de 2021.

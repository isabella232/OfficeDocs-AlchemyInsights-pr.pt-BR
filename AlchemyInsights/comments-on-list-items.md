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
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995465"
---
# <a name="comments-on-list-items"></a>Comentários sobre itens de lista

Os usuários podem exibir todos os comentários em um item de lista e filtrar entre exibições que mostram comentários ou atividades relacionadas a um item.

Os usuários precisam observar o seguinte antes de adicionar e excluir comentários:

- Os comentários seguem as configurações de permissão inerentes SharePoint.
- Listas clássicas que ainda não foram criadas para aparecer em interfaces de usuário modernas, como listas de tarefas, não terão esse recurso de comentário.
- Comentar as listas no Teams não está disponível com esta versão.
- Os comentários não são indexados pela Pesquisa.

Os administradores podem desabilitar esse recurso no nível da organização alterando o **parâmetro CommentsOnListItemsDisabled** no cmdlet **Set-SPOTenant** PowerShell.

No momento, não é possível desabilitar o comentário no nível do site ou da lista. Esperamos ter esses controles em uma atualização posterior, provavelmente no primeiro trimestre de 2021.

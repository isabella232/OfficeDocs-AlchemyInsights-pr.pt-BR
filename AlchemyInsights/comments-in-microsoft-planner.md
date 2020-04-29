---
title: Comentários no Microsoft Planner
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 98246b52e21c7a24d04e18ce77d96b28c65e7909
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911208"
---
# <a name="comments-in-microsoft-planner"></a>Comentários no Microsoft Planner

Os comentários das tarefas em um plano são armazenados na caixa de correio do Exchange Online para o Grupo do Microsoft 365 associado ao plano.  Quando você publica um comentário em uma tarefa, uma notificação por email é enviada para a caixa de entrada do grupo e você recebe um email por cada comentário subsequente feito nessa tarefa.

Aqui estão algumas respostas para problemas comuns relacionados aos comentários:

- **Os usuários não estão recebendo emails** - Os comentários são enviados para a caixa de entrada do grupo ao qual o plano pertence. Para que um usuário receba emails do grupo, o grupo deve estar configurado para enviar conversas do grupo para as caixas de entrada dos membros.

- **Os comentários não estão sendo salvos** - O usuário que adiciona o comentário não tem permissão para enviar emails ao grupo do Microsoft 365. Leia [Como o Microsoft Planner Funciona](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) para obter mais informações sobre esse cenário.

- O erro **Você não tem mais acesso** é exibido ou **os usuários convidados não podem adicionar comentários** - Usuários convidados que não podem enviar email para a caixa de entrada do grupo podem ver esta mensagem. Para resolver, verifique se o usuário convidado possui um endereço de email válido.

- **Usuários removidos estão recebendo emails** - Se um usuário comentar sobre uma tarefa antes de ser removido do plano, o thread de email incluirá o usuário para cada comentário feito na tarefa.

Para obter informações detalhadas sobre comentários no Microsoft Planner, confira [como o Microsoft Planner funciona](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) e [Comentário em tarefas no Microsoft Planner](https://support.microsoft.com/office/comment-on-tasks-in-microsoft-planner-fd4aedde-7785-4cd0-96ee-122fbc9140e1).

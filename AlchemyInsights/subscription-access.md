---
title: Acesso à assinatura
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773767"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Não é possível entrar no Azure devido a problemas de navegador (o navegador trava, continua girando, não carrega, etc.)

Você pode ser afetado por uma interrupção. Verifique se há uma interrupção em andamento: [status de integridade do Azure](https://status.azure.com/status/history/).

Faça logoff de todas as sessões ativas do Azure. Inicie um modo in-private ou incógnito do navegador da Web.

Você também pode tentar atualizar o navegador, usar outro navegador, Excluir cookies de cache se acima não funcionar.

Saiba mais: [solucionar problemas de entrada](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Não é possível acessar assinaturas**

No [portal do Azure](https://portal.azure.com/), certifique-se de que o diretório do Azure correto está selecionado na conta no canto superior direito.

No [centro de contas do Azure](https://account.windowsazure.com/Subscriptions), certifique-se de que a conta usada seja o administrador da conta.

Saiba mais: [solucionar problemas de nenhuma assinatura encontrada](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Não é possível acessar o histórico de cobrança**

O administrador da conta precisa certificar-se de que o usuário que estiver acessando as informações de cobrança seja adicionado ao Azure Active Directory como um usuário convidado: [Adicionar ou excluir um novo usuário](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Em seguida, o usuário deve receber uma função de administrador global: [atribuir função aos usuários](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Postar isso, o usuário pode receber acesso de cobrança usando políticas RBAC: [conceder acesso à cobrança](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos Recomendados**

-   [Não consigo entrar para gerenciar minha assinatura do Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)
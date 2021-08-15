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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999228"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Não é possível entrar no Azure devido a problemas do navegador (o navegador trava, continua girando, não carrega, etc.)

Você pode ser afetado por uma paralisação. Verifique se há uma paralisação contínua: Status de [Saúde do Azure.](https://status.azure.com/status/history/)

Faça logon de todas as sessões ativas do Azure. Inicie um modo in-private ou incógnito do navegador da Web.

Você também pode tentar Atualizar navegador, usar outro navegador, excluir cookies de cache se acima não funcionar.

Saiba mais: Solucionar [problemas de login](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Não é possível acessar assinaturas**

No [portal do Azure,](https://portal.azure.com/)certifique-se de que o diretório correto do Azure está selecionado na conta no canto superior direito.

No Centro [de Conta do Azure,](https://account.windowsazure.com/Subscriptions)certifique-se de que a conta usada seja o administrador da conta.

Saiba mais: [Solução de problemas sem assinaturas encontradas](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Não é possível acessar o histórico de cobrança**

O administrador da conta precisa garantir que o usuário que acessa as informações de cobrança seja adicionado ao Azure Active directory como um usuário convidado: Adicionar ou [excluir um novo usuário](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Em seguida, o usuário precisa receber uma função de administrador global: [Atribuir função aos usuários](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Poste isso, o usuário pode receber acesso de cobrança usando políticas do RBAC: [Conceder acesso à cobrança](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos Recomendados**

-   [Não posso entrar para gerenciar minha assinatura do Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)
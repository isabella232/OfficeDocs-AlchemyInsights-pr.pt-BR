---
title: Como adicionar e gerenciar os administradores-etapas recomendadas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755823"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Como adicionar e gerenciar os administradores-etapas recomendadas

Com base na descrição do problema, encontramos uma solução para você. A maioria dos clientes foi capaz de resolver seu problema por conta própria após seguir nossa documentação.

**Editar o administrador de assinaturas ou coadministrador**

- O administrador da conta pode editar as duas funções, enquanto o administrador de assinaturas só pode alterar os coadministradores no [portal do Azure](https://ms.portal.azure.com/#home).
- [Adicionar ou alterar administradores de assinatura do Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Atualizar o administrador de assinaturas ou Co-Administrator para assinaturas internas (TRANSMITIdas)**

O administrador de serviço ou o coadministrador pode atender a essa ação usando as seguintes etapas:

1. Faça logon no [portal do Azure](https://ms.portal.azure.com/#home) e clique em **Gerenciamento de custos + cobrança** na folha esquerda.
2. Clique no item de linha com sua assinatura. Isso abre a visão geral da sua assinatura.
3. Na folha **assinatura** , clique em **Propriedades**. 
4. Clique no botão **administrador de serviços** .
5. Insira o email do usuário que você deseja definir como administrador de serviço e clique em **OK**.

**Adicionar/Alterar/remover coadministrador**

1. Faça logon no [portal do Azure](https://ms.portal.azure.com/#home) como um administrador de serviço.
2. Abra [assinaturas](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) e selecione uma assinatura. (Coadministradores só podem ser atribuídos no escopo de assinatura.)
3. Navegue até **controle de acesso (iam)**  >  **os administradores clássicos**  >  **Add**  >  **Add coadministrador** para abrir o painel **Adicionar** coadministrador (se a opção Adicionar coadministrador estiver desabilitada, ela indica que você não tem permissões).
4. Selecione o usuário que você deseja adicionar e clique em **Adicionar**.

**Saiba Mais:**
- [Adicionar um coadministrador](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Remover um coadministrador](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Alterar o administrador de serviço](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Exibir o administrador da conta](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gerenciar o acesso usando o RBAC e o portal do Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Adicionar/excluir usuários usando o Azure Active Directory (AD)**

Você pode adicionar novos usuários ou excluir usuários existentes da organização do Azure Active Directory (Azure AD):

1. Para adicionar um novo usuário, faça logon no [portal do Azure](https://ms.portal.azure.com/#home) como administrador de usuário da organização.
2. Selecione **Azure Active Directory**, selecione **usuários** e, em seguida, clique em **novo usuário**.
3. Na página do **usuário** , preencha as informações necessárias. Clique em **Criar**. O usuário é criado e adicionado ao seu locatário do Azure AD.

**Saiba mais**:

- [Adicionar um novo usuário](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Excluir um usuário](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Adicionar ou atualizar as informações de perfil de um usuário usando o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documentos recomendados**

- [O que é controle de acesso baseado em função (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Entender as diferentes funções no Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Permissões da função de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Tutorial: conceder acesso a um usuário usando o RBAC e o portal do Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Solucionar problemas de RBAC no Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizar seus recursos com grupos de gerenciamento do Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Como solicitar a cópia da fatura do Azure via email](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Como adicionar, atualizar ou remover um cartão de crédito ou débito do Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Gerenciar a assinatura (reativar/cancelar/alternar)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




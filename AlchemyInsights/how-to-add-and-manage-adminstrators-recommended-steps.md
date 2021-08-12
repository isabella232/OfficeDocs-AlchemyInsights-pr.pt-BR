---
title: Como adicionar e gerenciar administradores - etapas recomendadas
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
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963775"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Como adicionar e gerenciar administradores - etapas recomendadas

Com base na descrição do problema, encontramos uma solução para você. A maioria dos clientes conseguiu resolver seus problemas por conta própria após seguir nossa documentação.

**Editar o Administrador de Assinatura ou Co-administrador**

- O Administrador de Conta pode editar ambas as funções, enquanto o Administrador de Assinatura só pode alterar Co-administradores no [portal do Azure.](https://ms.portal.azure.com/#home)
- [Adicionar ou alterar administradores de assinatura do Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Atualizar o Administrador de Assinatura ou Co-Administrator para Assinaturas Internas (AIRS)**

O Administrador de Serviços ou o Co-administrador podem auto-atender a essa ação usando as seguintes etapas:

1. Faça logoff no [portal do Azure](https://ms.portal.azure.com/#home) e clique em **Gerenciamento de Custos + Cobrança** na folha esquerda.
2. Clique no item de linha com sua assinatura. Isso abre a visão geral da sua assinatura.
3. Na folha **Assinatura,** clique em **Propriedades**. 
4. Clique no **botão Administrador do** Serviço.
5. Insira o email do usuário que você deseja definir como administrador de serviço e clique em **OK**.

**Add/Change/Remove Co-administrator**

1. Faça logoff no [portal do Azure](https://ms.portal.azure.com/#home) como Administrador de Serviços.
2. Abra [Assinaturas](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) e selecione uma assinatura. (Os co-administradores só podem ser atribuídos no escopo da assinatura.)
3. Navegue até Controle de Acesso **(IAM)** Administradores clássicos Adicione Adicionar co-administrador para abrir o painel Adicionar  >    >    >   **co-administrador** (Se a opção Adicionar co-administrador estiver desabilitada, ela indica que você não tem permissões).
4. Selecione o usuário a quem você deseja adicionar e clique em **Adicionar**.

**Saiba Mais:**
- [Adicionar um Co-Administrador](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Remover um co-administrador](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Alterar o Administrador de Serviços](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Exibir o Administrador de Conta](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gerenciar o acesso usando o RBAC e o portal do Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Adicionar/excluir usuários usando Azure Active Directory (AD)**

Você pode adicionar novos usuários ou excluir usuários existentes de sua organização Azure Active Directory (Azure AD) :

1. Para adicionar um novo usuário, faça logoff no [portal do Azure](https://ms.portal.azure.com/#home) como administrador do usuário da organização.
2. Selecione **Azure Active Directory,** selecione **Usuários** e clique em **Novo usuário**.
3. Na página **Usuário,** preencha as informações necessárias. Clique em **Criar**. O usuário é criado e adicionado ao locatário do Azure AD.

**Saiba mais**:

- [Adicionar um novo usuário](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Excluir um usuário](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Adicionar ou atualizar as informações de perfil de um usuário usando Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documentos Recomendados**

- [O que é o controle de acesso baseado em função (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Compreender as diferentes funções no Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Permissões da função de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Tutorial: conceder acesso a um usuário usando o RBAC e o portal do Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Solucionar problemas do RBAC no Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizar seus recursos com grupos de gerenciamento do Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Como solicitar cópia da fatura do Azure por email](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Como adicionar, atualizar ou remover um cartão de crédito ou débito do Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Gerenciar assinatura (Reativar/Cancelar/Alternar)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




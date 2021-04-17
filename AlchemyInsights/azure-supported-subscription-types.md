---
title: Tipos de assinatura com suporte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820670"
---
# <a name="supported-subscription-types"></a>Tipos de assinatura com suporte

Examine os tipos de assinatura com suporte para prosseguir.

[Tipos de assinatura com suporte](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Transferir propriedade de cobrança**

Portal do Azure como a [Administrador da Conta](https://ms.portal.azure.com/) de cobrança que tem a assinatura que você deseja transferir

- Pesquisar em **Custo de Gerenciamento + Faturamento**. Selecione **Assinaturas** no painel esquerdo. Dependendo do acesso, talvez seja necessário selecionar um escopo de cobrança e, em seguida, **Assinaturas** ou **Assinaturas do Azure**.
- Selecione Transferir propriedade de cobrança para a assinatura que você deseja transferir
- Insira o endereço de e-mail de um usuário que é administrador de cobrança da conta e será o novo proprietário da assinatura e selecione **enviar solicitação de transferência**
- O usuário recebe um email com instruções para revisar sua solicitação de transferência. Para aprovar a solicitação de transferência, o usuário seleciona o link no email e segue as instruções.

Observação: se você transferir a propriedade de cobrança da sua assinatura para uma conta de usuário em outro locatário do Azure AD, todos as atribuições de [controle de acesso baseado em função (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para gerenciamento de recursos na assinatura serão permanentemente removidas. Somente o novo proprietário terá acesso ao gerenciamento de recursos na assinatura. Para saber mais, confira [Transferindo a assinatura para um usuário em outro locatário do Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Transferir a Propriedade da Assinatura**

As funções de pré-requisitos baseados na Transferência de Propriedade Assinatura (RBAC) para gerenciar os recursos na assinatura perdem o acesso. Para obter mais informações sobre como adicionar uma assinatura existente a um locatário, confira [Associar ou adicionar uma assinatura do Azure ao Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- A Transferência de Assinatura com um valor pendente existente do ciclo de faturamento atual não será transferida para o novo instrumento de pagamento na nova conta. A única informação disponível para os usuários na nova conta é o custo do mês anterior para a sua assinatura. O restante do histórico de uso e cobrança não é transferido para a assinatura.
- A transferência de propriedade de cobrança das assinaturas do Enterprise Agreement (EA) só tem suporte no portal do Enterprise Agreement
- Transferir uma assinatura orientada por crédito, como a do Visual Studio, BizSpark, Microsoft Partner Network para um novo usuário exige que uma licença do Visual Studio/Microsoft Partner Network aceite a solicitação de transferência
- Todos os recursos, como Máquinas Virtuais, discos e sites, são transferidos para a nova conta com êxito. Os seguintes recursos podem ser afetados em uma transferência de assinatura entre os locatários:

**Azure AD Domain Services**

Azure Key Vaults

- [Usuários e bancos de dados relacionados ao SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) podem ser afetados, especialmente se o cliente usa uma autenticação relativa do Azure Active Directory.
- **Os serviços de aplicativo** configurados com a autenticação do Azure Active Directory poderiam ser afetados
- As contas do **Visual Studio Team** Services conectadas a assinaturas do Azure podem perder temporariamente o acesso quando a assinatura do Azure conectada é cancelada

**Documentos Recomendados**

Etapas após aceitar a propriedade de cobrança:

- Para manter a propriedade da cobrança, mas alterar o tipo de sua assinatura, confira: [Mudar sua assinatura do Azure para outra oferta](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transferindo Visual Studio, Microsoft Partner Network (MPN) e assinaturas pré-pagas de desenvolvimento/teste](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transferir a propriedade de cobrança das assinaturas do Enterprise Agreement (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Perguntas frequentes sobre Transferência de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Solucionar problemas de Transferência de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
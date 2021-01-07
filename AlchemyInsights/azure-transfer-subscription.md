---
title: Transferir propriedade de cobrança do Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 74b7cc879973790b7532106c80b718856682a334
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755535"
---
# <a name="transfer-azure-billing-ownership"></a>Transferir propriedade de cobrança do Azure

Entre no [portal do Azure](https://portal.azure.com/) como administrador da conta de cobrança que possui a assinatura que deseja transferir. Se você não tiver certeza se é um administrador ou se precisa determinar quem é, confira [Determinar o administrador de cobrança da conta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Pesquise por _Gerenciamento de Custos + Cobrança_.
1. Selecione **Assinaturas** no painel esquerdo. Dependendo do acesso, você pode precisar selecionar um escopo de cobrança e, em seguida, **Assinaturas** ou **Assinaturas do Azure**.
1. Selecione **Transferir propriedade de cobrança** para a assinatura que deseja transferir.
1. Insira o endereço de email de um usuário que é administrador de cobrança da conta e será o novo proprietário da assinatura e selecione **enviar solicitação de transferência**.
1. O usuário recebe um email com instruções para revisar sua solicitação de transferência. Para aprovar a solicitação de transferência, o usuário seleciona o link no email e segue as instruções.

Observe que se você transferir a propriedade de cobrança de sua assinatura para uma conta de usuário em outro locatário do Azure Active Directory, todas as atribuições de [controle de acesso baseado em função (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para gerenciar recursos na assinatura serão permanentemente removido. Somente o novo proprietário terá acesso ao gerenciamento de recursos na assinatura. Para obter mais informações sobre como alterar o diretório de uma assinatura, confira [Transferindo a assinatura para um usuário em outro locatário do Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Impacto importante nas suas faturas**_: se você tiver transferido a propriedade da cobrança de uma assinatura do Azure, suas cobranças serão classificadas como um profissional. Você poderá acessar as faturas conforme o seguinte:  

1. Selecione sua assinatura na  [página Assinaturas](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) no portal do Azure como  [um usuário com acesso a faturas](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) e selecione  **Faturas**.
1. Clique em  **Baixar Fatura**  para exibir uma cópia de sua fatura em PDF. Se disser  _Não disponível_, confira  [Por que não vejo a fatura do último período de cobrança?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. Você também pode exibir o seu uso diário clicando no **período de cobrança** para obter um PDF de sua fatura e uma cópia do arquivo detalhado de uso diário (.CSV) Para saber mais, confira  [Obter dados de uso de faturas](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos Recomendados**

- [Transferir a propriedade de cobrança de uma assinatura do Azure para outra conta](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Sobre a transferência de propriedade de cobrança para uma assinatura do Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transferindo o Microsoft Visual Studio, Microsoft Partner Network (MPN) e assinaturas de desenvolvimento/teste Pré-pagos](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Perguntas frequentes sobre Transferência de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Solucionar problemas de Transferência de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

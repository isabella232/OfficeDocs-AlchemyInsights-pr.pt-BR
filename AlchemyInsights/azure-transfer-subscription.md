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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840566"
---
# <a name="transfer-azure-billing-ownership"></a>Transferir propriedade de cobrança do Azure

Entre no [portal do Azure](https://portal.azure.com/) como administrador da conta de cobrança que possui a assinatura que deseja transferir. Se não tiver certeza se você é o administrador ou se precisa determinar quem é, confira [Determinar o administrador de cobrança da conta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Pesquise em **Gerenciamento de Custos + Cobrança**.
- Selecione **Assinaturas** no painel esquerdo. Dependendo do acesso, você pode precisar selecionar um escopo de cobrança e, em seguida, **Assinaturas** ou **Assinaturas do Azure**.
- Selecione **Transferir propriedade de cobrança** para a assinatura que deseja transferir
- Insira o endereço de e-mail de um usuário que é administrador de cobrança da conta e será o novo proprietário da assinatura e selecione **enviar solicitação de transferência**
- O usuário recebe um email com instruções para revisar sua solicitação de transferência. Para aprovar a solicitação de transferência, o usuário seleciona o link no email e segue as instruções.

**Observação** : Se você transferir a propriedade de cobrança de sua assinatura para uma conta de usuário em outro locatário do Azure Active Directory, todas as atribuições de [controle de acesso baseado em função (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para gerenciar recursos na assinatura serão permanentemente removido. Somente o novo proprietário terá acesso ao gerenciamento de recursos na assinatura. Para saber mais, confira [Transferindo a assinatura para um usuário em outro locatário do Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos Recomendados**

- [Transferir a propriedade de cobrança de uma assinatura do Azure para outra conta](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Sobre a transferência de propriedade de cobrança para uma assinatura do Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transferindo o Microsoft Visual Studio, Microsoft Partner Network (MPN) e assinaturas de desenvolvimento/teste Pré-pagos](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Perguntas frequentes sobre Transferência de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Solucionar problemas de Transferência de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

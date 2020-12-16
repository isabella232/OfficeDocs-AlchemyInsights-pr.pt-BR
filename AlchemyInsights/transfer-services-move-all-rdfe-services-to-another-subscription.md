---
title: Serviços de transferência-mover todos os serviços RDFE para outra assinatura
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681446"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Serviços de transferência-mover todos os serviços RDFE para outra assinatura

**Mover recursos**

Os recursos do Azure podem ser movidos para outra assinatura do Azure ou grupo de recursos na mesma assinatura usando o portal do Azure, o Azure PowerShell, o Azure CLI ou a API REST para mover recursos.

Antes de poder mover recursos, consulte:

- [Lista de verificação antes de mover os recursos](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Serviços que podem ser movidos](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Como validar a movimentação](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Diretrizes de movimentação para serviços](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Para mover recursos existentes para outro grupo de recursos ou assinatura, você pode usar:

- [Portal do Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [CLI do Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [mover recursos do Azure para outro grupo de recursos ou assinatura](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Solucionar erros com o Azure Resource Manager**

Consulte os artigos abaixo para saber mais sobre alguns erros comuns de implantação do Azure e receber informações para resolvê-los. Se você não conseguir encontrar o código de erro para o erro de implantação, confira [Localizar código de erro](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Solucionar erros de implantação](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Solucionar problemas de movimentação de recursos do Azure para o novo grupo de recursos ou assinatura](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Observe que, se você quiser atualizar sua assinatura do Azure, como mudar de gratuita para pagar conforme o ponto, precisará converter sua assinatura.

- Para atualizar uma avaliação gratuita, confira [atualizar sua assinatura de avaliação gratuita ou Microsoft imagine Azure para o pagamento conforme a ser acessado](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Para alterar uma conta de pagamento conforme você, confira [alterar sua assinatura de pagamento a ser direcionado do Azure para uma oferta diferente](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Para adicionar ou associar uma assinatura do Azure ao seu locatário do Azure Active Directory:**

1. Entre e selecione a assinatura que você deseja usar na [página assinaturas no portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Selecione **Alterar diretório**.
3. Revise todos os avisos exibidos e selecione **alterar**.
4. O diretório é alterado para a assinatura e você receberá uma mensagem de êxito.
5. Use o seletor de *diretório* para ir para o novo diretório. Pode levar até 10 minutos para que tudo seja exibido corretamente.

**Documentos Recomendados**

- [Transferindo a propriedade de uma assinatura do Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mover recursos para o novo grupo de recursos ou assinatura](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gerenciar recursos usando o portal do Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)

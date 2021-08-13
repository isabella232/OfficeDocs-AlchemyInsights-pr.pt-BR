---
title: Serviços de Transferência - Mover todos os serviços RDFE para outra assinatura
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940020"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Serviços de Transferência - Mover todos os serviços RDFE para outra assinatura

**Mover recursos**

Os recursos do Azure podem ser movidos para outra assinatura ou grupo de recursos do Azure sob a mesma assinatura usando o portal do Azure, Azure PowerShell, Azure CLI ou a API REST para mover recursos.

Antes de mover recursos, consulte:

- [Lista de verificação antes de mover recursos](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Serviços que podem ser movidos](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Como validar a movimentação](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Mover diretrizes para serviços](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Para mover recursos existentes para outro grupo de recursos ou assinatura, você pode usar:

- [Portal do Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [Mover recursos do Azure para outro grupo de recursos ou assinatura](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Solucionar erros com o Gerenciador de Recursos do Azure**

Consulte os artigos abaixo para saber mais sobre alguns erros comuns de implantação do Azure e receber informações para resolvê-los. Se você não conseguir encontrar o código de erro do erro de implantação, consulte [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Solucionar erros de implantação](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Solucionar problemas de movimentação de recursos do Azure para novo grupo de recursos ou assinatura](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Observe que, se você quiser atualizar sua assinatura do Azure, como alternar de gratuito para pago conforme você vai, você precisará converter sua assinatura.

- Para atualizar uma avaliação gratuita, consulte [Upgrade your Free Trial or Microsoft Imagine assinatura do Azure to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Para alterar uma conta pay-as-you-go, consulte [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Para adicionar ou associar uma assinatura do Azure ao seu Azure Active Directory locatário:**

1. Entre e selecione a assinatura que você deseja usar na página [Assinaturas no portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Selecione **Alterar diretório**.
3. Revise os avisos que aparecem e selecione **Alterar**.
4. O diretório é alterado para a assinatura e você receberá uma mensagem de sucesso.
5. Use o *comutor* de diretório para ir para o novo diretório. Pode levar até 10 minutos para tudo aparecer corretamente.

**Documentos Recomendados**

- [Transferindo a propriedade de uma assinatura do Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mover recursos para novo grupo de recursos ou assinatura](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gerenciar recursos usando o portal do Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)

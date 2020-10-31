---
title: Cobrança para compra de Instância Reservada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815965"
---
# <a name="billing-for-reserved-instance-purchase"></a>Cobrança para compra de Instância Reservada

A compra da instância reservada é cobrada pelo método de pagamento vinculado à assinatura selecionada no momento da compra. O tipo de assinatura deve ser um contrato empresarial (número da oferta: MS-AZR-0017P), Pagamento Conforme o Uso (número da oferta: MS-AZR-0003), Contrato de Cliente da Microsoft ou CSP.

- Para uma assinatura empresarial, os encargos são deduzidos do saldo do compromisso monetário da inscrição ou cobrados como excedente
- Para uma assinatura de Pagamento Conforme o Uso, os encargos são cobrados no cartão de crédito ou como fatura da assinatura

**Cancelar Reserva**

- **Autoatendimento:** cancele ou troque uma instância reservada usando o [portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Escolha a reserva e clique em reembolso ou troca. Observe que é necessário ter acesso de proprietário no Pedido de Reserva para fazer reembolso ou troca. Somente o acesso à Reserva não permitirá que você faça reembolso ou troca. Solicite ao proprietário do Pedido de Reserva o acesso de proprietário ao Pedido de Reserva
- **Política de troca:** você pode trocar uma reserva por outra do mesmo tipo; **não há penalidades** na troca de reserva. O compromisso total com a nova reserva deve ser maior que a soma do valor de reembolso da reserva trocada e os pagamentos mensais futuros (se aplicável)
- **Política de reembolso:** a soma do reembolso e os pagamentos futuros cancelados não podem exceder US$ 50.000 em um intervalo de 12 meses. **No momento, não cobramos nenhuma multa** em reembolsos, mas poderá ser cobrado em reembolsos futuros

**Exceções:** a troca de autoatendimento e a capacidade de cancelamento não estão disponíveis para clientes do US Government Enterprise Agreement

- O suporte para **API/PS/CLI** não está disponível para cancelamento e reembolsos [Trocas de autoatendimento e reembolsos para Reservas do Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- A troca de autoatendimento e a capacidade de cancelamento não estão disponíveis para clientes do US Government Enterprise Agreement. Outros tipos de assinatura do Governo dos EUA, incluindo Pré-pago e CSP, têm suporte

Saiba mais: [como as transações de retorno e do Exchange são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) saiba mais: [políticas do Exchange e de reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) outras perguntas: [visitar documentos de instância reservado](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Trocar uma instância reservada existente (autoatendimento)**

Você pode trocar uma reserva por outra reserva do mesmo tipo. Você também pode reembolsar uma reserva, até US$ 50.000 por ano, caso não precise mais dela. A troca de autoatendimento e a capacidade de cancelamento não estão disponíveis para clientes do US Government Enterprise Agreement. Outros tipos de assinatura do Governo dos EUA, incluindo Pré-pago e CSP, têm suporte. É necessário ter acesso de proprietário no Pedido de Reserva para fazer reembolso ou troca de uma reserva existente.

As etapas a seguir orientarão sobre o procedimento para concluir a transação

1. faça logon no [portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecione as reservas que você deseja restituir e clique em **Exchange** 2. Selecione o produto da VM que você deseja comprar e digite uma quantidade. Certifique-se de que o novo total de compra seja maior do que o total de retorno [determina o tamanho certo antes da compra](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. revise e conclua a transação

**Reembolso de uma instância reservada**

Para reembolsar uma reserva, vá para **Detalhes da Reserva** e clique em **Reembolso**

**Reembolso proporcional:**

**Ration e exemplos de requisitos mínimos para restituição e troca** Exemplo de reserva upfront:

- Você compra um RI com prazo de um ano por US$ 120 em 1 de janeiro
- Em 7 de abril você deseja reembolsar ou trocar essa reserva
- Como a reserva ficou ativa por 97 dias, você receberá (1-97/365)* US$ 120 de volta. (por exemplo, US$ 88,1). No momento, não há nenhuma multa em reembolsos
- Se você trocar, a nova compra deve ser maior do que US$ 88,1
- Não há, no momento, nenhuma multa em reembolsos

**Exemplo de reserva de plano de cobrança:**

- Você compra um RI com prazo de um ano por US$ 10 mensais
- Em 7 de abril você deseja reembolsar ou trocar essa reserva
- Como o último pagamento ocorreu há sete dias, você receberá (1-7/31) * US$ 10 de volta. (por exemplo, US$ 7,74)
- Os pagamentos futuros cancelados são de US$ 80. No momento, não há nenhuma multa em reembolsos
- Esse cancelamento deduzirá US$ 87,74 do seu limite de reembolso US$ 50.000
- Se você trocar, o valor total da nova compra deve ser maior do que US$ 87,74

**Não é possível ver a fatura para o último período de cobrança**

Algumas possíveis razões pelas quais você pode não ver uma fatura:

- Você tem um valor de crédito mensal com sua assinatura que você não ultrapassou ou tem uma avaliação gratuita. Uma fatura só é gerada quando você deve ser dinheiro
- É menos de 30 dias do dia em que você se inscreveu no Azure
- A fatura ainda não é gerada. Aguardar até o final do período de cobrança
- Se você não for o administrador da conta, as faturas antigas podem não estar disponíveis para você

**Baixar sua fatura do portal do Azure (. pdf)**

- Selecione sua assinatura na página [assinaturas](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) no portal do Azure como [um usuário com acesso a faturas](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selecionar **faturas**
- Clique em **baixar fatura** para exibir uma cópia da fatura do PDF. Se ele disser **não estiver disponível** , confira [por que não vejo uma fatura para o último período de cobrança?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Receber sua fatura em email (. pdf)**

- Selecione sua assinatura na página [assinaturas](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Clique em **faturas** e enviar minha fatura
- Clique **em aceitar e** aceite os termos. Você precisará aceitar todas as assinaturas de sua propriedade

Observação: se você não receber um email após seguir as etapas, verifique se o seu endereço de email está correto nas [preferências de comunicação no seu perfil](https://account.windowsazure.com/profile)

**Baixar os dados de uso do portal do Azure**

- Entre no [centro de contas do Azure](https://account.windowsazure.com/Subscriptions) como [administrador da conta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selecione a assinatura para a qual você deseja as informações de uso e fatura
- Selecionar **histórico de cobrança**
- Selecione **Exibir instrução atual** para ver uma estimativa de seus encargos no momento em que a previsão foi gerada
- Selecione **baixar o uso** para baixar os dados de uso diário como um arquivo CSV. Se você vir duas versões disponíveis, baixe a versão 2

Outras questões: [acesse o documentos de instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos Recomendados**

- [Noções básicas de cobrança](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entender como o desconto de instância reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Baixar ou exibir sua fatura do Azure cobrança e dados de uso diário](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entender como o desconto de instância reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entender o uso da instância reservada para sua assinatura de pagamento conforme a ser direcionado](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entender o uso da instância reservada para o registro corporativo](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Custos de software do Windows não incluídos em instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instâncias reservadas no programa provedor de soluções de nuvem central (CSP) de parceiro](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)
---
title: Cobrança para compra de Instância Reservada
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104008"
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

Saiba mais : [Como as](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) transações de retorno e de troca são processadas Saiba mais [:](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Exchange e políticas de reembolso Outras perguntas: Visite documentos de instância [reservada](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Trocar uma instância reservada existente (autoatendimento)**

Você pode trocar uma reserva por outra reserva do mesmo tipo. Você também pode reembolsar uma reserva, até US$ 50.000 por ano, caso não precise mais dela. A troca de autoatendimento e a capacidade de cancelamento não estão disponíveis para clientes do US Government Enterprise Agreement. Outros tipos de assinatura do Governo dos EUA, incluindo Pré-pago e CSP, têm suporte. É necessário ter acesso de proprietário no Pedido de Reserva para fazer reembolso ou troca de uma reserva existente.

As etapas a seguir orientarão sobre o procedimento para concluir a transação

1.Faça logoff no portal [do Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selecione as reservas que você deseja reembolsar e clique em **Exchange** 2.Selecione o produto VM que deseja comprar e digite uma quantidade. Certifique-se de que o novo total de compra seja maior do que o total de retorno [Determine o tamanho certo antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Revise e conclua a transação

**Reembolso de uma instância reservada**

Para reembolsar uma reserva, vá para **Detalhes da Reserva** e clique em **Reembolso**

**Reembolso proporcional:**

**Pro de ração e requisitos mínimos para reembolso e troca** Exemplo de reserva inicial:

- Você compra um RI com prazo de um ano por US$ 120 em 1º de janeiro
- Em 7 de abril você deseja reembolsar ou trocar essa reserva
- Como a reserva ficou ativa por 97 dias, você receberá (1-97/365)* US$ 120 de volta. (por exemplo, US$ 88,1). No momento, não há nenhuma multa em reembolsos
- Se você trocar, a nova compra deverá ser maior do que US$ 88,1
- Não há, no momento, nenhuma multa em reembolsos

**Exemplo de reserva de plano de cobrança:**

- Você compra um RI com prazo de um ano por US$ 10 mensais
- Em 7 de abril você deseja reembolsar ou trocar essa reserva
- Como o último pagamento ocorreu há sete dias, você receberá (1-7/31) * US$ 10 de volta. (por exemplo, US$ 7,74)
- Os pagamentos futuros cancelados são de US$ 80. No momento, não há nenhuma multa em reembolsos
- Esse cancelamento deduzirá US$ 87,74 do seu limite de reembolso US$ 50.000
- Se você trocar, o valor total da nova compra deverá ser maior do que US$ 87,74

**Não é possível ver a fatura do último período de cobrança**

Alguns motivos possíveis para você não ver uma fatura:

- Você tem um valor de crédito mensal com sua assinatura que não excedeu ou tem uma avaliação gratuita. Uma fatura só é gerada quando você deve dinheiro
- São menos de 30 dias a partir do dia em que você se inscreve no Azure
- A fatura ainda não foi gerada. Aguarde até o final do período de cobrança
- Se você não for o Administrador de Conta, as faturas mais antigas podem não estar disponíveis para você

**Baixe sua fatura do portal do Azure (.pdf)**

- Selecione sua assinatura na página [Assinaturas](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) no portal do Azure como [um usuário com acesso a faturas](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selecionar **Faturas**
- Clique em **Baixar Fatura** para exibir uma cópia de sua fatura em PDF. Se disser **Não disponível**, confira [Por que não vejo a fatura do último período de cobrança?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Receber sua fatura por email (.pdf)**

- Selecione sua assinatura na página [Assinaturas.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Clique **em Faturas,** em seguida, Envie um email para minha fatura
- Clique **em Aceitar** e aceite os termos. Você terá que optar por cada assinatura que possuir

Observação: se você não receber um email após seguir as etapas, certifique-se de que seu endereço de email está correto nas [preferências](https://account.windowsazure.com/profile) de comunicação em seu perfil

**Baixar seus dados de uso do portal do Azure**

- Entrar no [Centro de Conta do Azure](https://account.windowsazure.com/Subscriptions) como Administrador de [Conta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selecione a assinatura para a qual você deseja a fatura e as informações de uso
- Selecionar **Histórico de Cobrança**
- Selecione **Exibir instrução Current** para ver uma estimativa de suas cobranças no momento em que a estimativa foi gerada
- Selecione **Baixar Uso** para baixar os dados de uso diários como um arquivo CSV. Se você vir duas versões disponíveis, baixe a versão 2

Outras questões: [acesse os documentos de instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos Recomendados**

- [Noções básicas de cobrança](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entenda como o desconto de Instância Reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Baixar ou exibir sua fatura de cobrança do Azure e dados de uso diários](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entenda como o desconto de Instância Reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entender o uso da Instância Reservada para sua assinatura Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entender o uso da Instância Reservada para seu registro Enterprise registro](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows de software não incluídos em instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instâncias reservadas no programa de Provedor de Soluções na Nuvem (CSP) do Partner Central](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)
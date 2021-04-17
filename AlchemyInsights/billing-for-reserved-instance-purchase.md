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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820310"
---
# <a name="billing-for-reserved-instance-purchase"></a>Cobrança para compra de Instância Reservada

A compra de instância reservada é cobrada ao método de pagamento vinculado à assinatura selecionada no momento da compra. O tipo de assinatura deve ser um contrato empresarial (número de oferta: MS-AZR-0017P), Pay-As-You-Go (número de oferta: MS-AZR-0003P), Contrato de Cliente da Microsoft ou CSP.

- Para uma assinatura corporativa, os encargos são deduzidos do saldo de compromisso monetário do registro ou cobrados como excesso
- Para a assinatura Pay-As-You-Go, os encargos são cobrados no cartão de crédito ou no método de pagamento da fatura na assinatura

**Cancelando Reserva**

- **Self-service:** Você mesmo pode cancelar ou trocar uma instância reservada usando [o portal do Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selecione a reserva e clique em reembolso ou no exchange. Observe que você deve ter acesso ao proprietário na Ordem de Reserva para troca ou reembolso. O acesso somente à Reserva não permitirá que você prossiga com reembolso ou troca. Peça ao proprietário do Pedido de Reserva para lhe dar acesso ao Pedido de Reserva
- **Política do Exchange:** Você pode trocar uma reserva por outra reserva do mesmo tipo – não há **penalidades** na troca de reserva. O compromisso total com a nova reserva deve ser maior do que a soma do valor de reembolso da reserva trocada e os pagamentos mensais futuros (se aplicável)
- **Política de reembolso:** A soma do reembolso e os pagamentos futuros cancelados não podem exceder US$ 50.000 em uma janela de rolagem de 12 meses. No **momento, não estamos cobrando nenhuma penalidade** sobre reembolsos, mas podemos cobrar por reembolsos futuros

**Exceções:** A funcionalidade de troca e cancelamento de autoatend Contrato Enterprise eua

- **O suporte à API/PS/CLI** não está disponível para cancelamento e reembolsos de trocas e reembolsos de autoatendência para Reservas [do Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- A funcionalidade de troca e cancelamento de autoatendado não está disponível para clientes Contrato Enterprise Us Government. Outros tipos de assinatura do Governo dos EUA, incluindo Pay-As-You-Go e CSP, são suportados

Saiba mais : [Como as transações](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) de retorno e de troca são processadas Saiba mais : Políticas [de Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) e Reembolso Outras perguntas: Visite documentos de instância [reservada](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange an existing reserved instance (Self-service)**

Você pode trocar uma reserva por outra reserva do mesmo tipo. Você também pode reembolsar uma reserva, até US$ 50.000 por ano, se não precisar mais dela. A funcionalidade de troca e cancelamento de autoatendado não está disponível para clientes Contrato Enterprise Us Government. Outros tipos de assinatura do Governo dos EUA, incluindo Pay-As-You-Go e CSP, são suportados. Você deve ter acesso ao proprietário na Ordem de Reserva para trocar ou reembolsar uma reserva existente.

As etapas a seguir orientarão sobre o procedimento para concluir a transação

1.Faça logoff no portal [do Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selecione as reservas que você deseja reembolsar e clique em **Exchange** 2.Selecione o produto VM que deseja comprar e digite uma quantidade. Certifique-se de que o novo total de compra seja maior do que o total de retorno [Determine o tamanho certo antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Revise e conclua a transação

**Reembolso de uma instância reservada**

Para reembolsar uma reserva, acesse **Detalhes da Reserva** e clique em **Reembolso**

**Reembolso proporcional:**

**Exemplos de requisitos mínimos e pro-rações para reembolso e troca** Exemplo de reserva inicial:

- Você compra uma RI de um ano por US$ 120 em 1º de janeiro
- Em 7 de abril, você deseja reembolsar ou trocar essa reserva
- Como a reserva foi ao vivo por 97 dias, você receberá (1-97/365) * US$ 120 de volta. (ou seja, US$ 88,1). No momento, não há nenhuma penalidade sobre reembolsos
- Se a troca for trocada, sua nova compra deverá ser maior do que US$ 88,1
- No momento, não há nenhuma penalidade sobre reembolsos

**Exemplo de reserva do plano de cobrança:**

- Você compra uma RI de um ano por US$ 10 por mês
- Em 7 de abril, você deseja reembolsar ou trocar essa reserva
- Como o último pagamento ocorreu por 7 dias, você receberá (1 a 7/31) * R$ 10 de volta. (ou seja, $7,74)
- Os pagamentos futuros cancelados são de US$ 80. No momento, não há nenhuma penalidade sobre reembolsos
- Esse cancelamento deduzirá US$ 87,74 do limite de reembolso de US$ 50.000
- Se a troca for trocada, o valor total da nova compra deve ser maior do que US$ 87,74

**Não é possível ver a fatura do último período de cobrança**

Alguns motivos possíveis para você não ver uma fatura:

- Você tem um valor de crédito mensal com sua assinatura que não excedeu ou tem uma avaliação gratuita. Uma fatura só é gerada quando você deve dinheiro
- São menos de 30 dias a partir do dia em que você se inscreve no Azure
- A fatura ainda não foi gerada. Aguarde até o final do período de cobrança
- Se você não for o Administrador de Conta, as faturas mais antigas podem não estar disponíveis para você

**Baixe sua fatura do portal do Azure (.pdf)**

- Selecione sua assinatura na página [Assinaturas](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) no portal do Azure como [um usuário com acesso a faturas](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selecionar **Faturas**
- Clique em **Baixar Fatura** para exibir uma cópia de sua fatura em PDF. Se ele diz **Não disponível**, consulte Por que não vejo uma fatura para o último período [de cobrança?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

Outras perguntas: [Visite documentos de instância reservada](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos Recomendados**

- [Noções básicas de cobrança](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entenda como o desconto de Instância Reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Baixar ou exibir sua fatura de cobrança do Azure e dados de uso diários](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entenda como o desconto de Instância Reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entender o uso da Instância Reservada para sua assinatura Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Compreender o uso da Instância Reservada para seu registro empresarial](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Custos de software do Windows não incluídos em instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instâncias reservadas no programa CSP (Provedor de Soluções de Nuvem Central de Parceiros)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)
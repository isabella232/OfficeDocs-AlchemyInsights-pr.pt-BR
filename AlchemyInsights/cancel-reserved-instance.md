---
title: Cancelar Reserva
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819680"
---
# <a name="cancelling-reservation"></a>Cancelar Reserva

- **Autoatendimento:** cancele ou troque uma instância reservada usando o [portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Escolha a reserva e clique em reembolso ou troca. Observe que é necessário ter acesso de proprietário no Pedido de Reserva para fazer reembolso ou troca. Somente o acesso à Reserva não permitirá que você faça reembolso ou troca. Solicite ao proprietário do Pedido de Reserva o acesso de proprietário ao Pedido de Reserva
- **Política de troca:** você pode trocar uma reserva por outra do mesmo tipo; **não há penalidades** na troca de reserva. O compromisso total com a nova reserva deve ser maior que a soma do valor de reembolso da reserva trocada e os pagamentos mensais futuros (se aplicável)
- **Política de reembolso:** a soma do reembolso e os pagamentos futuros cancelados não podem exceder US$ 50.000 em um intervalo de 12 meses. **No momento, não cobramos nenhuma multa** em reembolsos, mas poderá ser cobrado em reembolsos futuros  
    **Exceções:** a troca de autoatendimento e a capacidade de cancelamento não estão disponíveis para clientes do US Government Enterprise Agreement
- O suporte para **API/PS/CLI** não está disponível para cancelamento e reembolsos [Trocas de autoatendimento e reembolsos para Reservas do Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- A troca de autoatendimento e a capacidade de cancelamento não estão disponíveis para clientes do US Government Enterprise Agreement. Outros tipos de assinatura do Governo dos EUA, incluindo Pré-pago e CSP, têm suporte

Saiba mais: [como as transações de devolução e de troca são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Saiba mais: [políticas de Troca e de Reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Outras questões: [acesse os documentos de instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Trocar uma instância reservada existente (autoatendimento)**

Você pode trocar uma reserva por outra reserva do mesmo tipo. Você também pode reembolsar uma reserva, até US$ 50.000 por ano, caso não precise mais dela. A troca de autoatendimento e a capacidade de cancelamento não estão disponíveis para clientes do US Government Enterprise Agreement. Outros tipos de assinatura do Governo dos EUA, incluindo Pré-pago e CSP, têm suporte. É necessário ter acesso de proprietário no Pedido de Reserva para fazer reembolso ou troca de uma reserva existente.

As etapas a seguir orientarão sobre o procedimento para concluir a transação

1. Entre no [portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Escolha as reservas que deseja reembolsar e clique em **Troca**
2. Escolha o produto de VM que deseja comprar e digite uma quantidade. Verifique se o novo total da compra é maior do que o total da devolução [Determinar o tamanho correto antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Revisar e concluir a transação

**Reembolso de uma instância reservada**

Para reembolsar uma reserva, vá para **Detalhes da Reserva** e clique em **Reembolso**

**Reembolso proporcional:**

**Exemplos de proporcionais e requisitos mínimos para reembolso e troca**  
Exemplo de reserva antecipada:

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

**Documentos Recomendados**

- [Como as transações de devolução e de troca são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Políticas de Troca e de Reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)
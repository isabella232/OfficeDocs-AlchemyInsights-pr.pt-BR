---
title: Por que o botão Adicionar orçamento está desabilitado para mim?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822623"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Por que o botão Adicionar orçamento está desabilitado para mim?

Para criar um orçamento, você precisa de uma das seguintes permissões:

- Grupo de Gerenciamento, Assinatura, Escopos de Grupo de Recursos
- Colaborador de Gerenciamento de Custos
- Proprietário
- Colaborador
- Somente cliente corporativo: Registro, departamento, escopos de conta
- Administrador de Registro (definir orçamento no escopo de inscrição)
- Administrador do Departamento (definir orçamento no escopo do Departamento)
- Proprietário da conta (definir orçamento no escopo da conta)
- Contrato de Cliente Moderno Somente: Conta de Cobrança, Perfil de Cobrança, Escopos da Seção Fatura
- Criador de assinaturas do Azure

**Criei um orçamento quando meu custo para o mês atual já estava acima do orçamento. Por que não recebi um alerta?**  
Se você já excedeu um determinado limite de custo ao criar um orçamento que o alerta não disparará. Quando um novo ciclo começar, se você violar o limite, o alerta será a disparar.

**Quando devo esperar receber um alerta depois de exceder um dos limites de alerta de orçamento definidos?**  
Os orçamentos são avaliados a cada 4 horas. Leva no mínimo 8 horas para que os dados de uso cheguem ao sistema de orçamentos. Devido a isso, os alertas podem levar até 12 horas para disparar depois que você exceder um limite.

**Por que o botão Data de início está desabilitado quando seleciono um período de redefinição de mês ou de cobrança?**  
Os orçamentos são alinhados ao mês do calendário atual ou ao período de cobrança atual (no caso em que o Mês de Cobrança está selecionado). Portanto, preenchemos previamente esse valor para você.

**Por que não vejo um gráfico dos meus custos na experiência de criação de orçamento?**  
Precisamos de no mínimo 2 meses de dados de custo para poder renderizar um gráfico para ajudá-lo com a criação de orçamento.

**Por que não posso definir um orçamento em relação a uma assinatura que acabei de criar?**  
Após a criação de uma assinatura, os dados demoram de 24 a 48 horas para processar antes de definir um orçamento em relação a ela.

**Recursos da API de Orçamento**

- [API de orçamentos v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): fornece operações para criar e atualizar orçamentos. Usando a API orçamentos, você pode definir um limite de orçamento e configurar vários alertas para disparar à medida que se aproxima desse limite. Os alertas podem disparar um email ou um Grupo de Ações do Azure para executar a automação. Observação: a filtragem dessa API não se alinha com a filtragem/dimensões da API de consulta.
- [API de orçamentos v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Criar orçamentos com recursos de filtragem de custos maiores do que v1. A filtragem se alinha ao contrato usado em nossas APIs de Consulta e Dimensões. Esta é a API de orçamentos recomendada para usar o avançar.
- [Dimensões](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): fornece operações para obter dimensões com suporte para seu uso em uma variedade de escopos. Usando a API dimensões, você pode recuperar uma lista de dimensões que podem ser usadas como entradas para gerar consultas com a API de Consulta.
- [Consulta](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): fornece operações para obter dados agregados de custo e uso com base na consulta que você fornece. Usando a API de Consulta, você pode especificar sua filtragem, classificação e agrupação desejadas em todas as dimensões disponíveis (que são acessadas a partir da API dimensões).

**Custos previstos**

**Por que não vejo previsões para meus custos na Análise de Custo?**  
Há vários motivos pelos quais a projeção de previsão pode estar ausente para você na Análise de Custo, algumas delas são as seguintes:

1. Se seus dados de custo têm menos de 10 dias, o gráfico de previsão não será carregado. O modelo requer pelo menos 10 dias de dados de custo recentes para projeções precisas
2. Se você tiver selecionado datas históricas, o gráfico de previsão não ficará visível. Selecione um intervalo de datas com datas futuras para que o gráfico de previsão seja exibido
3. Se sua conta tiver várias moedas, o gráfico de previsão só projetará custos para 'Todos os custos em USD'

**Por que a previsão não muda quando faço alterações nos meus recursos?**  
O modelo de previsão requer alguns dias para levar em conta as alterações na conta e não faz projeções imediatas com base na alteração nos recursos  
Para etapas maiores de aumento ou diminuição de recursos, o modelo levará um pouco mais de tempo para se ajustar a essas alterações para levar em conta as anomalias

**Por que minha previsão aumenta depois que faço uma reserva ou uma compra do Marketplace?**  
O modelo de previsão considera seu "Custo Real" e não conta com o uso e a compra separadamente. Para uma compra única, o modelo diminuirá as projeções após 10 dias para levar em conta o aumento repentino dos custos

**Quero ver previsões para uma única dimensão (por exemplo. Medidor)**  
A previsão atualmente dá suporte a projeções de custo total e não para medidores individuais. Portanto, quando 'Agrupada por' uma dimensão, as projeções serão para o total de todos os itens na dimensão

**Documentos Recomendados**

- [O que é o Gerenciamento de Custos do Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Práticas recomendadas de Gerenciamento de Custos do Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analisar seus custos e gastos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorar e analisar custos com análise de custo](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gerenciamento de Custos do Azure: Preços](https://azure.microsoft.com/services/cost-management/#pricing)
- [Analisar custos na análise de custo](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial em vídeo: criar um orçamento no portal do Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Pré-requisitos para exibição e personalização de orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Criar e gerenciar orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurar a automação com a API de Grupos de Ações e Orçamentos do Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Usar alertas de custo para monitorar o uso e os gastos](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Práticas recomendadas de Gerenciamento de Custos](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vídeos de tutoriais**

- [Criar um orçamento no portal do Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gerenciar custos com a API de Orçamentos e grupos de ações](https://go.microsoft.com/fwlink/?linkid=2147038)
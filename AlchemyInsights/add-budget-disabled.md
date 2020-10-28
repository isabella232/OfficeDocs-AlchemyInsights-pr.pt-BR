---
title: Por que o botão Adicionar orçamento está desabilitado para mim?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48769585"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Por que o botão Adicionar orçamento está desabilitado para mim?

Para criar um orçamento, você precisa de uma das seguintes permissões:

- Grupo de gerenciamento, assinatura, escopos de grupo de recursos
- Contribuidor de gerenciamento de custos
- Proprietário
- Colaborador
- Somente cliente corporativo: registro, departamento, escopos de conta
- Administrador de registro (definir orçamento no escopo de registro)
- Administrador do departamento (definir orçamento no escopo do departamento)
- Proprietário da conta (definir orçamento no escopo da conta)
- Apenas o contrato de cliente moderno: conta de cobrança, perfil de cobrança, escopos de seção de fatura
- Criador de assinatura do Azure

**Criei um orçamento quando o custo do mês atual já estava acima do orçamento. Por que não recebi um alerta?**  
Se você já excedeu um determinado limite de custo quando cria um orçamento que o alerta não será acionado. Após o início de um novo ciclo, se você violar o limite, o alerta será acionado.

**Quando deve-se esperar receber um alerta depois que eu exceder um dos meus limites de alerta de orçamento definidos?**  
Os orçamentos são avaliados a cada quatro horas. É necessário um mínimo de 8 horas para que os dados de uso atinjam o sistema de orçamentos. Assim, os alertas podem levar até 12 horas para serem acionados depois que você exceder um limite.

**Por que o botão de data de início é desabilitado quando eu seleciono um mês ou um período de redefinição de mês de cobrança?**  
Os orçamentos são alinhados ao mês do calendário atual ou ao período de cobrança atual (no caso em que mês de faturamento estiver selecionado). Portanto, preenchemos esse valor para você.

**Por que não vejo um gráfico dos meus custos na experiência de criação de orçamento?**  
Precisamos de um mínimo de 2 meses de dados de custo para que possamos renderizar um gráfico para ajudá-lo com a criação de orçamento.

**Por que não posso definir um orçamento com uma assinatura que acabei de criar?**  
Após a criação de uma assinatura, os dados levam 24-48 horas para serem processados antes de definir um orçamento para ele.

**Recursos de API de orçamento**

- [Orçamentos API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): fornece operações para criar e atualizar orçamentos. Usando a API de orçamentos, você pode definir um limite de orçamento e configurar vários alertas para serem acionados conforme você abordar o limite. Os alertas podem disparar um email ou um grupo de ações do Azure para executar a automação. Observação: a filtragem para esta API não é alinhada à filtragem/dimensões de API de consulta.
- [Orçamentos API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Crie orçamentos com recursos de filtragem de custo mais avançados do que o v1. A filtragem se alinha ao contrato usado em nossas APIs de consulta e dimensões. Essa é a API de orçamentos recomendada para usar a movimentação para frente.
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): fornece operações para obter as dimensões suportadas para o uso em vários escopos. Usando a API de dimensões, você pode recuperar uma lista de dimensões que podem ser usadas como entradas para gerar consultas com a API de consulta.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): fornece operações para obter dados agregados de custo e uso com base na consulta que você fornecer. Usando a API de consulta, você pode especificar a filtragem, classificação e agrupamento desejados em todas as dimensões disponíveis (que são acessadas a partir da API de dimensões).

**Custos previstos**

**Por que não vejo previsões de meus custos na análise de custos?**  
Há várias razões pelas quais a previsão de projeção pode estar ausente para você na análise de custos, algumas delas são as seguintes:

1. Se os dados de custo tiverem menos de 10 dias, o gráfico de previsão não será carregado. O modelo requer pelo menos 10 dias de dados de custo recentes para projeções precisas
2. Se você tiver selecionado datas históricas, o gráfico de previsão não estará visível. Selecione um intervalo de datas com datas futuras para que o gráfico de previsão seja exibido
3. Se sua conta tiver várias moedas, o gráfico de previsão só projetará os custos de "todos os custos em USD"

**Por que a previsão não muda quando faço alterações nos meus recursos?**  
O modelo de previsão requer alguns dias para considerar as alterações na conta e não faz projeções imediatas com base na alteração dos recursos  
Para maiores etapas de aumento ou redução dos recursos, o modelo levará um pouco mais para se ajustar às alterações feitas em conta de anomalias

**Por que minha previsão aumenta após fazer uma reserva ou compra de Marketplace?**  
O modelo de previsão considera o ' custo real ' e não conta o uso e a compra separadamente. Para uma compra única, o modelo diminuirá as projeções após 10 dias para considerar o aumento repentino nos custos

**Desejo ver previsões para uma única dimensão (por exemplo, Métrica**  
A previsão atualmente oferece suporte a projeções de custo total e não para medidores individuais. Portanto, quando ' agrupado por ' uma dimensão, as projeções serão para o total de todos os itens na dimensão

**Documentos Recomendados**

- [O que é o gerenciamento de custos do Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Práticas recomendadas de gerenciamento de custos do Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analisar custos e despesas](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorar e analisar custos com a análise de custos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gerenciamento de custos do Azure: preços](https://azure.microsoft.com/services/cost-management/#pricing)
- [Analisar custos na análise de custo](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial de vídeo: criar um orçamento no portal do Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Pré-requisitos para exibir e personalizar orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Criar e gerenciar orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurar a automação com o Azure Action Groups e a API de orçamentos](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Usar alertas de custo para monitorar o uso e gastos](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Práticas recomendadas de gerenciamento de custos](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vídeos de tutorial**

- [Criar um orçamento no portal do Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gerenciar custos com a API de orçamentos e grupos de ações](https://go.microsoft.com/fwlink/?linkid=2147038)
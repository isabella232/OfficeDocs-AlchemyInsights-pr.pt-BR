---
title: Configurando o serviço provisionamento
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033266"
---
# <a name="configuring-the-provision-service"></a>Configurando o serviço provisionamento

Para que o provisionamento de usuário automatizado funcione, o Azure AD requer credenciais válidas que permitem que ele se conecte à API de Serviços Web do Workday. Além disso, o botão Conexão de Teste no aplicativo Workday to AD User Provisioning também valida se ele é capaz de se conectar ao Agente de Provisionamento do Azure AD Conexão associado ao Domínio do AD.

Se o portal do Azure estiver retornando um erro ao salvar as credenciais, siga as etapas recomendadas abaixo:

1. Confirme se você configurou a conta de usuário do Sistema de Integração do Workday conforme indicado na seção tutorial Configurar o usuário do sistema de integração [no Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Confirme se o Serviço de Agente de Provisionamento Conexão Azure AD está em execução em seu servidor local Windows usando o Console de Gerenciamento de Serviços. Você também pode verificar o status do agente no portal do Azure clicando no botão Exibir agentes locais.
3. Certifique-se de que você está inserindo o valor do campo "Nome do Usuário do Dia de Trabalho" usando o formato username@workday nome do locatário. Se o nome do locatário do dia de trabalho estiver ausente, a autenticação workday falhará.
4. Se você estiver configurando a integração com o locatário de implementação do Workday, anote os horários de inatividade agendados do locatário do Workday. Workday programou o tempo de inatividade para seus locatários de implementação nos finais de semana (geralmente de sexta à noite até sábado de manhã) e falhas de conectividade durante essa janela de tempo de inatividade é um problema conhecido que resolve automaticamente assim que os locatários de implementação estão novamente online.
5. Em casos raros, você também poderá ver esse erro se a senha do Usuário do Sistema de Integração for alterada devido à atualização do locatário ou se a conta estiver bloqueada ou expirada. Verifique o status do usuário do Sistema de Integração com o administrador do Workday.

Para obter mais detalhes sobre como configurar o Workday para provisionamento automatizado, confira [Tutorial: Configurar o Workday para provisionamento automático](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

---
title: O Workday para o Provisionamento de Usuário do AD entra em estado de quarentena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036480"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>O Workday para o Provisionamento de Usuário do AD entra em estado de quarentena

**O Workday para o Provisionamento de Usuário do AD entra em estado de quarentena e nenhum usuário é criado no AD**

O Workday para o trabalho do Provisionamento de Usuário do AD foi para o estado de quarentena e os logs de auditoria mostram os eventos de falha de exportação com a mensagem de erro **Error: OperationsError-SvcErr: Ocorreu um erro de operação. Nenhuma referência superior foi configurada para o serviço de diretório. O serviço de diretório, portanto, não pode emitir referências a objetos fora desta floresta**. Esse erro normalmente aparece se o UO do Contêiner do Active Directory não estiver configurado corretamente ou se houver problemas com o Expression Mapping usado para **parentDistinguishedName**.

Verifique se há erros de digitação no parâmetro UO Padrão para **Novos Usuários**. Verifique se o UO especificado já existe no seu AD. Se você estiver usando **parentDistinguishedName** no mapeamento de atributos, verifique se ele sempre avalia para um recipiente conhecido dentro do domínio do AD. Verifique o evento Exportar nos logs de auditoria para ver o valor gerado.

Para obter mais detalhes sobre como configurar o Workday para provisionamento automatizado, confira [Tutorial: Configurar o Workday para provisionamento automático](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).


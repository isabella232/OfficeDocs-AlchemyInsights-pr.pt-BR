---
title: Problemas com o filtro de atributo e o de escopo
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
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430710"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problemas com o filtro de atributo e o de escopo

**Problema com valores UPN conflitantes**

O Workday para o AD User Provisioning Workday to AD User Provisioning mostra a mensagem de erro **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. A operação falhou porque o valor UPN fornecido para adição/modificação não é exclusivo para toda a floresta. Detalhes do Erro: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

O valor **userPrincipalName** que o conector Workday tenta definir ao criar a conta de usuário do AD já existe no domínio do AD de destino. Isso implica que (1) o usuário já existe e a verificação de ID correspondente falhou para o usuário ou (2) a regra de geração de UPN gerou um valor conflitante.

Veja as etapas de resolução sugeridas:

Se o usuário já existe e a verificação de ID correspondente não conseguiu vincular a conta Workday à conta do Active Directory, então verifique se o atributo do ID correspondente (geralmente, **employeeID**) no Workday e no AD têm uma correspondência exata. Se eles não corresponderem, será necessário corrigir algum problema existente nos dados. Por exemplo, se o EmployeeID no Workday for 001052, e no AD for 1052, então o mecanismo de provisionamento falhará ao vincular as duas contas e tentará criar um usuário já existente. A solução neste caso é alterar o valor **EmployeeID** no AD para incluir os zeros à esquerda e deixá-lo como 001052.
Se a expressão geradora de UPN não gerar um valor exclusivo, considere o uso da função de eliminação de duplicação **SelectUniqueValue** para gerar um valor exclusivo a cada vez.

**O Workday para o AD User Provisioning não define o valor do atributo gerente para a conta de usuário do AD**

O Workday para o trabalho do AD User Provisioning não define o valor do atributo **manager** para as contas de usuários do AD. Há dois cenários possíveis quando esse comportamento acontece:

1. O gerenciador no Workday não pode ser resolvido para uma conta de usuário do AD correspondente, pois o gerenciador não está no escopo.
2. Em um cenário de **vários domínios do AD**, o gerenciador no Workday não está presente no mesmo domínio que o usuário.

Tente seguir estas etapas para resolver o problema:

1. Se você definiu os filtros de escopo, verifique primeiro se o gerenciador está no escopo e se ele atende a cláusula de escopo. Se o gerenciador não atender ao filtro de escopo, altere o filtro para que o gerenciador também esteja no escopo da operação de provisionamento.
2. Se você tiver vários domínios do AD, o conector terá uma limitação conhecida como a incapacidade de resolver referências do gerenciador de domínios cruzados.

Para obter mais detalhes sobre como configurar o Workday para provisionamento automatizado, confira [Tutorial: Configurar o Workday para provisionamento automático](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).














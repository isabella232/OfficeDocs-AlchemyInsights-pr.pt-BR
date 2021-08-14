---
title: Privileged Identity Management função
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973217"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) role

**As permissões não são concedidas após a ativação de uma função**

Quando você ativa uma função no Azure AD Privileged Identity Management (PIM), a ativação pode não se propagar instantaneamente para todos os portais que exigem a função privilegiada. Às vezes, mesmo que a alteração seja propagada, o cache da Web em um portal pode resultar na alteração não entrar em vigor imediatamente.

Se a ativação for adiada, siga estas etapas:

1. Saia do portal do Azure e entre novamente. Ao ativar uma função do Azure AD ou uma função de recurso do Azure, você verá os estágios de sua ativação. Depois que todos os estágios são concluídos, você verá um link "Sair". Você pode usar esse link para sair. Isso resolverá a maioria dos casos de atraso na ativação.
2. No PIM, verifique se você está listado como o membro da função.
3. Se você estiver ativando a função Exchange Administrador, certifique-se de sair e entrar novamente. Se o problema persistir, abra um tíquete de suporte e eleva isso como um problema. Se você estiver usando sua função Exchange administrador para acessar o Centro de Segurança e Conformidade, consulte a próxima etapa.
4. Se você estiver ativando uma função para acessar o Centro de Conformidade e Segurança ou se estiver ativando a função de administrador do SharePoint, você terá algum atraso de ativação de alguns minutos até algumas horas. Esse é um problema conhecido e estamos trabalhando ativamente com essas equipes para resolver esse problema assim que possível.

Para saber mais, confira:

- [Ativar minhas funções do Azure AD no PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Ativar minhas funções de recurso do Azure no PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**As permissões não são removidas após a desativação de uma função ou a ativação de função expira**

Quando você desativa uma função no Azure AD Privileged Identity Management ou quando um período de ativação de função expira, pode haver um atraso em que você continue a ter acesso.

Se sua desativação for adiada, siga estas etapas:

1. Se você estiver desativando a função de administrador do Exchange ou o período de ativação de função expirar e perceber um atraso significativo antes de as permissões ser removidas, abra um tíquete de suporte e diga ao engenheiro de suporte para ajudá-lo a registrar um tíquete com a equipe de Gerenciamento de Acesso Privilegiado (PAM) dentro Office sobre esse problema.
2. Se o período de ativação tiver expirado, mas você ainda tiver a sessão do navegador aberta, feche o navegador. Você pode continuar a usar a função até fechar essa sessão. Esse é um problema conhecido e estamos procurando uma correção potencial para revogar ativamente cada sessão depois que a ativação expirar.

Se o atraso for diferente desses dois cenários, abra um tíquete de suporte.

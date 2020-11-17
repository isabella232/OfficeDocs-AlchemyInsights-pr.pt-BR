---
title: Função de gerenciamento de identidade privilegiada
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086198"
---
# <a name="privileged-identity-managementpim-role"></a>Função de gerenciamento de identidade privilegiada (PIM)

**As permissões não são concedidas após a ativação de uma função**

Quando você ativa uma função no Azure AD Privileged Identity Management (PIM), a ativação pode não ser propagada instantaneamente para todos os portais que exigem a função privilegiada. Às vezes, mesmo que a alteração seja propagada, o cache da Web em um portal pode fazer com que a alteração não tenha efeito imediato.

Se a ativação estiver atrasada, siga estas etapas:

1. Saia do portal do Azure e entre novamente. Ao ativar uma função do Azure AD ou uma função de recurso do Azure, você verá os estágios da ativação. Depois que todos os estágios forem concluídos, você verá um link de "desconexão". Você pode usar esse link para sair. Isso resolverá a maioria dos casos de atraso de ativação.
2. No PIM, verifique se você está listado como o membro da função.
3. Se você estiver ativando a função de administrador do Exchange, certifique-se de sair e entrar novamente. Se o problema persistir, abra um tíquete de suporte e aumente isso como um problema. Se você estiver usando a função de administrador do Exchange para acessar o centro de segurança e conformidade, consulte a próxima etapa.
4. Se você estiver ativando uma função para acessar o centro de segurança e conformidade ou se estiver ativando a função de administrador do SharePoint, você terá um atraso de ativação de alguns minutos até algumas horas. Esse é um problema conhecido e estamos trabalhando ativamente com essas equipes para resolver esse problema o mais rápido possível.

Para saber mais, confira:

- [Ativar minhas funções do Azure AD no PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Ativar minhas funções de recurso do Azure no PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**As permissões não são removidas após a desativação de uma função ou a ativação da função expira**

Quando você desativa uma função no Azure AD Privileged Identity Management ou quando um período de ativação de função expira, pode haver um atraso para você continuar a ter acesso.

Se a desativação estiver atrasada, siga estas etapas:

1. Se você estiver desativando a função de administrador do Exchange ou se o período de ativação da função expirar, e você notar um atraso significativo antes de as permissões serem removidas, abra um tíquete de suporte e informe o engenheiro de suporte para ajudá-lo a arquivar uma permissão com a equipe de gerenciamento de acesso privilegiado (PAM) no Office sobre esse problema.
2. Se o período de ativação tiver expirado, mas você ainda tiver a sessão do navegador aberta, feche o navegador. Você pode continuar a usar a função até fechar essa sessão. Esse é um problema conhecido e estamos examinando uma possível correção para revogar ativamente cada sessão, uma vez que a ativação tenha expirado.

Se o seu atraso for diferente desses dois cenários, abra um tíquete de suporte.

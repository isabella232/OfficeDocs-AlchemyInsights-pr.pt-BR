---
title: Notificação do AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897402"
---
# <a name="notification-aad-connect"></a>Notificação do AAD Connect

- Certifique-se de que você está autorizado a executar a operação. Os administradores globais têm acesso por padrão. Além disso, você pode usar [o Controle de Acesso Baseado em Função para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar a permissão de registro ao Colaborador.
- Verifique se os pontos de extremidade necessários estão habilitados e não bloqueados devido ao firewall. Para obter detalhes, consulte [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- O registro pode falhar devido à comunicação de saída estar sujeita à inspeção SSL pela camada de rede.
- Certifique-se de ter verificado as configurações de notificação para o Azure AD Connect Health e revise sua configuração. Para entender como configurar as configurações de notificação para notificações de Saúde do Azure AD Connect, consulte este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Para saber mais sobre o relatório de sincronização do AAD Connect Health e como baixá-lo, consulte Relatório de [sincronização](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)de nível de objeto .

Para solucionar problemas de alertas de saúde do AAD Connect, siga o guia de solução de problemas para alertas de atratividade de dados do AAD Connect Health e para perguntas [frequentes,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) consulte [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).

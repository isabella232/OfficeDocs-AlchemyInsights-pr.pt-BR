---
title: Notificação do AAD Conexão
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
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097294"
---
# <a name="notification-aad-connect"></a>Notificação do AAD Conexão

- Certifique-se de que você está autorizado a executar a operação. Os administradores globais têm acesso por padrão. Além disso, você pode usar [o Controle de Acesso Baseado em Função para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar a permissão de registro ao Colaborador.
- Verifique se os pontos de extremidade necessários estão habilitados e não bloqueados devido ao firewall. Para obter detalhes, consulte [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- O registro pode falhar devido à comunicação de saída estar sujeita à inspeção SSL pela camada de rede.
- Certifique-se de ter verificado as configurações de notificação do Azure AD Conexão Health e revise sua configuração. Para entender como configurar as configurações de notificação para as notificações do Azure AD Conexão de saúde, consulte este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Para saber mais sobre o relatório de sincronização do AAD Conexão Health e como baixá-lo, consulte Relatório de [sincronização](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)de nível de objeto .

Para solucionar problemas de alertas de Conexão de saúde do [AAD,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) siga o guia de solução de problemas para alertas de atratividade de dados do AAD Conexão e para perguntas frequentes, consulte [Common AAD Conexão Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).

---
title: Corrigir política de locatário (substituição de ação)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552250"
---
# <a name="fix-tenant-policy-action-override"></a>Corrigir política de locatário (substituição de ação)

Uma política anti-spam em seu locatário afetou essa mensagem. Para revisar a política, faça o seguinte:

1. Vá para o Centro de Conformidade e Segurança [& do Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)e vá para Política de Gerenciamento de Ameaças   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Verifique se a origem **da** política indica o seguinte:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Em caso afirmado, na **guia Personalizado,** verifique as configurações da política que afetou a mensagem. É possível que as configurações **Padrão aplicadas** a todos os clientes da Proteção do Exchange Online afetaram a mensagem.

Para obter mais informações sobre como configurar políticas de filtro de spam, consulte [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).

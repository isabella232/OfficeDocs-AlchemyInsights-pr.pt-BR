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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034922"
---
# <a name="fix-tenant-policy-action-override"></a>Corrigir política de locatário (substituição de ação)

Uma política anti-spam em seu locatário afetou essa mensagem. Para revisar a política, faça o seguinte:

1. Vá para o [Centro Office 365 Segurança & Conformidade](https://go.microsoft.com/fwlink/p/?linkid=2077143)e vá para **Política** de Gerenciamento de Ameaças  >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Verifique se a origem **da** política indica o seguinte:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Em caso afirmado, na **guia Personalizado,** verifique as configurações da política que afetou a mensagem. É possível que as configurações **Padrão aplicadas** a todos os clientes Proteção do Exchange Online afetaram a mensagem.

Para obter mais informações sobre como configurar políticas de filtro de spam, consulte [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).

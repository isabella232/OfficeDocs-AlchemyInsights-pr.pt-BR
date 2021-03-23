---
title: Sobre administradores do Yammer
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
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995230"
---
# <a name="about-yammer-admins"></a>Sobre administradores do Yammer

**Administradores de rede**

Os administradores globais são promovidos automaticamente para a função Administrador Verificado em uma rede do Yammer. Nos seguintes casos, essa promoção pode não ocorrer corretamente:

- Várias redes do Yammer existem e o administrador está sendo assinado na rede errada. [A consolidação](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) de rede é necessária para chegar a uma rede do Yammer.
- O PIM do Azure está sendo usado. O usuário pode não ser promovido ao administrador global por tempo suficiente para que a promoção ocorra. Uma atualização futura para o Yammer pode resolver esse problema, mas é melhor promover os usuários para o administrador global manualmente.
- Existe um problema de sincronização com a rede do Yammer. Nesse caso, uma solicitação de suporte será necessária para investigação posterior.

Para obter mais informações sobre funções de administrador do Yammer, consulte [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Administradores de grupo**

Os administradores de grupo para grupos conectados do Microsoft 365 são sincronizados com a associação de grupo do Azure AD. Para grupos grandes, essa sincronização pode levar um longo período.

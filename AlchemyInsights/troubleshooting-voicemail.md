---
title: 'Solução de problemas de caixa postal '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: 36ba65c1ee67631a8b3c24c3407f46e3304541c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330732"
---
# <a name="troubleshooting-voicemail"></a>Solução de problemas de caixa postal

Verifique se o recurso Ocupado no Ocupado é intencional.

Se esse recurso não for necessário neste usuário:

1. Vá para [o Teams Admin center](https://admin.teams.microsoft.com/policies/calling).
1. No trilho esquerdo, navegue **políticas**  >  **de chamada de voz** Gerenciar  >  **políticas** na Política **de Chamada.**
1. Selecione **Gerenciar Usuários**.
1. Pesquise o usuário e altere a Política de Chamada para uma que tenha Ocupado ocupado está disponível **quando em** uma chamada para **Off**.
1. Clique em **Aplicar**.

**Observação**: as alterações nas políticas podem levar até 24 horas para ser replicadas.

Para obter mais informações sobre esse recurso, consulte: [Busy on Busy está disponível durante uma chamada](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).

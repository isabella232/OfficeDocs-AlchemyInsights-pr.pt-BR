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
ms.openlocfilehash: e639d74cd8dbbb03ffb5b253451c99c8fe639f024a46e173845a0f4d322e43ca
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972371"
---
# <a name="troubleshooting-voicemail"></a>Solução de problemas de caixa postal

Verifique se o recurso Ocupado no Ocupado é intencional.

Se esse recurso não for necessário neste usuário:

1. Vá para [o Teams Admin center](https://admin.teams.microsoft.com/policies/calling).
1. No trilho esquerdo, navegue **políticas**  >  **de chamada de voz** Gerenciar  >  **políticas** na Política **de Chamada.**
1. Selecione **Gerenciar Usuários**.
1. Pesquise o usuário e altere a Política de Chamada para uma que tenha Ocupado ocupado está disponível **quando em** uma chamada para **Off**.
1. Clique em **Aplicar**.
> [!NOTE]
> As alterações nas políticas podem levar até 24 horas para ser replicadas.

Para obter mais informações sobre esse recurso, consulte: [Busy on Busy está disponível durante uma chamada](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).

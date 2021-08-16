---
title: Corrigir regras de transporte
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034742"
---
# <a name="fix-transport-rules"></a>Corrigir regras de transporte

Uma regra de fluxo de emails personalizada afetou essa mensagem. Para revisar a regra exata, faça o seguinte:

1. Nos resultados do envio, em **Informações adicionais,** observe **o GUID** ou o Nome **da Política.**
2. Iniciar Exchange Shell de Gerenciamento. Para obter mais informações, [consulte Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Execute este comando (usando o GUID do envio):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Revise a descrição para ver as condições configuradas que afetaram a mensagem.

Para saber mais, confira [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).

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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568427"
---
# <a name="fix-transport-rules"></a>Corrigir regras de transporte

Uma regra de fluxo de emails personalizada afetou essa mensagem. Para revisar a regra exata, faça o seguinte:

1. Nos resultados do envio, em **Informações adicionais,** observe **o GUID** ou o Nome **da Política.**
2. Iniciar o Shell de Gerenciamento do Exchange. Para obter mais informações, [consulte Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Execute este comando (usando o GUID do envio):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Revise a descrição para ver as condições configuradas que afetaram a mensagem.

Para saber mais, confira [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).

---
title: Status do sensor de verificação do Ponto de Extremidade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: 903d64a59d3bf870572c3c643e3d9cb801b571cb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321063"
---
# <a name="defender-endpoint-check-sensor-status"></a>Status do sensor de verificação do Ponto de Extremidade

O bloco **Dispositivos com problemas de sensor** está localizado no painel Operações de Segurança. Este bloco fornece informações sobre a capacidade do dispositivo individual de fornecer dados do sensor e se comunicar com o serviço Ponto de Extremidade. Ele relata quantos dispositivos requerem atenção e ajuda a identificar dispositivos problemáticos e tomar medidas para corrigir os problemas conhecidos.

Dois indicadores de status no bloco fornecem informações sobre o número de dispositivos que não se reportam adequadamente ao serviço:

- Dispositivos **Misconfigured** que podem estar relatando dados do sensor parcialmente ao serviço de Ponto de Extremidade e podem ter erros de configuração que precisam ser corrigidos.
- Dispositivos **Inativos** que pararam de se reportar ao serviço de Ponto de Extremidade por mais de sete dias no mês anterior.

Clicar em qualquer um dos grupos direciona você para a lista de dispositivos, filtrada de acordo com suas escolhas. Na lista de dispositivos, você pode filtrar a lista de estado de integridade pelo seguinte status:

- Dispositivos **ativos** que estão se reportando ativamente ao serviço de Ponto de Extremidade.
- Dispositivos **Misconfigured** que podem estar relatando parcialmente os dados do sensor ao serviço de Ponto de Extremidade, mas têm erros de configuração que precisam ser corrigidos. Dispositivos mal configurados podem ter um ou uma combinação dos seguintes problemas:

    - Sem dados do sensor - os dispositivos pararam de enviar dados do sensor. Alertas limitados podem ser acionados a partir do dispositivo.
    - Comunicações prejudicadas: a capacidade de comunicação com o dispositivo está prejudicada. O envio de arquivos para análise profunda, bloqueio de arquivos, isolamento do dispositivo da rede e outras ações que exigem comunicação com o dispositivo podem não funcionar.
- Dispositivos **Inativos** que pararam de se reportar ao serviço de Ponto de Extremidade.

Você pode baixar a lista inteira em formato CSV usando o recurso Exportar.

Para obter mais informações, confira [Verificar o estado de integridade do sensor no Microsoft Defender para Ponto de Extremidade](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/check-sensor-status).

Para obter mais informações sobre o que fez com que um dispositivo ficasse inativo ou configurado incorretamente, confira [Corrigir sensores não íntegros no Microsoft Defender para Ponto de Extremidade](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).

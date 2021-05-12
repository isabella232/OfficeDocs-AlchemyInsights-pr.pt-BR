---
title: Problemas com a remoção de um dispositivo desligado ou desativado do Inventário de Dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319167"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemas com a remoção de um dispositivo desligado ou desativado do Inventário de Dispositivos

O Microsoft Defender para Ponto de Extremidade atualmente não permite remover manualmente o registro do dispositivo de um dispositivo desligado ou desativado do Inventário de Dispositivos.

Para fins de segurança, o dispositivo permanece no portal como um registro histórico por até 180 dias. No entanto, os dados do dispositivo são limpos de acordo com o período de retenção configurado.

**Observação:** Um dispositivo desligado ou desativado alterna automaticamente para o estado **Inativo** após sete dias. Além disso, os dispositivos que não estão ativos nos últimos 30 dias não são fatorados nos dados que refletem a pontuação de exposição a ameaças e gerenciamento de vulnerabilidades da sua organização ou a Pontuação Segura da Microsoft para Dispositivos.
 
Se você ainda não quiser ver determinados dispositivos no visualização Inventário de Dispositivos, tente colocar uma marca de dispositivo para filtrar o dispositivo desativado do ponto de vista Inventário de Dispositivos.

Para saber mais, confira:

[Dispositivos offboard do serviço Microsoft Defender para Ponto de Extremidade](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Pontuação de exposição no gerenciamento de ameaças e vulnerabilidades](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Corrigir sensores não salubres no Microsoft Defender para Ponto de Extremidade](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Como usar a marcação efetivamente (Parte 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Como usar a marcação efetivamente (Parte 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Como usar a marcação efetivamente (Parte 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)





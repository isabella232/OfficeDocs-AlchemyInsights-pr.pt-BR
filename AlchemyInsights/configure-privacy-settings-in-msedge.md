---
title: Configurar configurações de privacidade em Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090286"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Configurar configurações de privacidade em Microsoft Edge

Por padrão, se Microsoft Edge for implantado em plataformas que não Windows, os dados de diagnóstico e as informações do site não serão enviados à Microsoft. No entanto, se Microsoft Edge for implantado no Windows 10, os dados de diagnóstico e as informações do site serão enviados de acordo com as configurações de dados de diagnóstico Windows [usuários.](https://go.microsoft.com/fwlink/?linkid=2132472)

Para configurar como Microsoft Edge lida com a coleta de dados da sua organização, use as seguintes políticas de grupo:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) liga o relatório de uso e dados relacionados a falhas.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) envia informações de site usadas para melhorar serviços Microsoft.

Para saber mais, confira [Configurar configurações de política](https://go.microsoft.com/fwlink/?linkid=2132577).

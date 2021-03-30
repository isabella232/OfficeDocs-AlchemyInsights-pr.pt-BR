---
title: Configurar configurações de privacidade no Microsoft Edge
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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403773"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Configurar configurações de privacidade no Microsoft Edge

Por padrão, se o Microsoft Edge for implantado em plataformas que não sejam do Windows, os dados de diagnóstico e as informações do site não serão enviados à Microsoft. No entanto, se o Microsoft Edge for implantado no Windows 10, os dados de diagnóstico e as informações do site serão enviados de acordo com as configurações de dados de [Diagnóstico do Windows dos usuários.](https://go.microsoft.com/fwlink/?linkid=2132472)

Para configurar como o Microsoft Edge lida com a coleta de dados da sua organização, use as seguintes políticas de grupo:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) liga o relatório de uso e dados relacionados a falhas.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) envia informações de site usadas para melhorar os serviços da Microsoft.

Para saber mais, confira [Configurar configurações de política](https://go.microsoft.com/fwlink/?linkid=2132577).

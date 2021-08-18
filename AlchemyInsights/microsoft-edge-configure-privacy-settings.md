---
title: Microsoft Edge configurações de privacidade
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114160"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configurações de privacidade

Por padrão, se Microsoft Edge for implantado em plataformas que não Windows, os dados de diagnóstico e as informações do site não serão enviados à Microsoft. No entanto, se Microsoft Edge for implantado no Windows 10, os dados de diagnóstico e as informações do site serão enviados de acordo com as configurações de dados de diagnóstico Windows [usuários.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Para configurar como Microsoft Edge lida com a coleta de dados da sua organização, use as seguintes políticas de grupo:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Essa política permite o relatório de dados relacionados a falhas e uso.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Esta política envia informações de site que são usadas para melhorar serviços Microsoft.

Para saber mais, confira [Configurar configurações de política](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).
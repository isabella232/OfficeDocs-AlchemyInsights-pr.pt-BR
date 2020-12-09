---
title: Configurações de privacidade para configurar o Microsoft Edge
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599441"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Configurações de privacidade para configurar o Microsoft Edge

Por padrão, se o Microsoft Edge é implantado em plataformas que não são do Windows, dados de diagnóstico e informações de site não são enviados para a Microsoft. No entanto, se o Microsoft Edge estiver implantado no Windows 10, dados de diagnóstico e informações de site serão enviados de acordo com [as configurações de dados de diagnóstico do Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)dos usuários.

Para configurar como o Microsoft Edge manipula a coleta de dados para sua organização, use as seguintes políticas de Grupo:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): esta política permite o relatório de uso e dados relacionados à falha.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): esta política envia informações de site que são usadas para melhorar os serviços da Microsoft.

Para saber mais, confira [definir configurações de política](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).
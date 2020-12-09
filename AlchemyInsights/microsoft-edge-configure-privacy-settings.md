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
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="868c0-102">Configurações de privacidade para configurar o Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="868c0-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="868c0-103">Por padrão, se o Microsoft Edge é implantado em plataformas que não são do Windows, dados de diagnóstico e informações de site não são enviados para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="868c0-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="868c0-104">No entanto, se o Microsoft Edge estiver implantado no Windows 10, dados de diagnóstico e informações de site serão enviados de acordo com [as configurações de dados de diagnóstico do Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)dos usuários.</span><span class="sxs-lookup"><span data-stu-id="868c0-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="868c0-105">Para configurar como o Microsoft Edge manipula a coleta de dados para sua organização, use as seguintes políticas de Grupo:</span><span class="sxs-lookup"><span data-stu-id="868c0-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="868c0-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): esta política permite o relatório de uso e dados relacionados à falha.</span><span class="sxs-lookup"><span data-stu-id="868c0-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="868c0-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): esta política envia informações de site que são usadas para melhorar os serviços da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="868c0-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="868c0-108">Para saber mais, confira [definir configurações de política](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="868c0-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>
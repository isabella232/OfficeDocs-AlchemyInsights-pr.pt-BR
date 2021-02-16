---
title: Habilitar Dispositivo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255143"
---
# <a name="enable-device"></a><span data-ttu-id="fb7e8-102">Habilitar Dispositivo</span><span class="sxs-lookup"><span data-stu-id="fb7e8-102">Enable Device</span></span>

<span data-ttu-id="fb7e8-103">**Para habilitar o dispositivo usando o comando do Powershell**</span><span class="sxs-lookup"><span data-stu-id="fb7e8-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="fb7e8-104">Execute os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="fb7e8-104">Run the following commands:</span></span>

- <span data-ttu-id="fb7e8-105">Para obter o objeto device: `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="fb7e8-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="fb7e8-106">Para habilitar o dispositivo: `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="fb7e8-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="fb7e8-107">Para obter mais informações sobre como configurar o Hybrid Join em domínios gerenciados, consulte [Configurar o Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span><span class="sxs-lookup"><span data-stu-id="fb7e8-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>

---
title: Dispositivos do Gerenciador de Configurações ausentes no portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817232"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="4221b-102">Dispositivos do Gerenciador de Configurações ausentes no portal</span><span class="sxs-lookup"><span data-stu-id="4221b-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="4221b-103">Para que a sincronização do dispositivo funcione, os [pontos de extremidade de Internet necessários](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) devem estar acessíveis no servidor local que hospeda a função de Ponto de Conexão de Serviço.</span><span class="sxs-lookup"><span data-stu-id="4221b-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="4221b-104">Para solucionar problemas de sincronização de dispositivos, confira ao **CMGatewaySyncUploadWorker.log** localizado no ponto de conexão do serviço.</span><span class="sxs-lookup"><span data-stu-id="4221b-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="4221b-105">Saiba mais sobre [Anexação de locatário ao Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="4221b-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>

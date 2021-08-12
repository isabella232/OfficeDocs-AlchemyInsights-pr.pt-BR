---
title: Desabilitar a verificação de rede
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7e67a45b6f4d4b18f47ce55a0fde20f826498c5d25c4a6dec4311d8fe4c3735f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928537"
---
# <a name="disable-network-scan"></a>Desabilitar a verificação de rede

As verificações de compartilhamento de rede podem afetar o desempenho.  Para garantir que o cliente não digitalizar compartilhamentos/arquivos de rede por padrão, configure as seguintes configurações no aplicativo Windows Defender como **True**:

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles
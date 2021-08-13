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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966097"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Dispositivos do Gerenciador de Configurações ausentes no portal

Para que a sincronização do dispositivo funcione, os [pontos de extremidade de Internet necessários](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) devem estar acessíveis no servidor local que hospeda a função de Ponto de Conexão de Serviço. Para solucionar problemas de sincronização de dispositivos, confira ao **CMGatewaySyncUploadWorker.log** localizado no ponto de conexão do serviço.

Saiba mais sobre [Anexação de locatário ao Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).

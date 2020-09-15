---
title: Política de proteção de aplicativos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716881"
---
# <a name="application-protection-policy"></a>Política de proteção de aplicativos

Se você não tiver experiência com as políticas de proteção de aplicativo (APP), confira o [Visão geral das políticas de proteção de aplicativo](https://docs.microsoft.com/intune/apps/app-protection-policy).

Para começar a usar o aplicativo, consulte [Como criar e atribuir políticas de proteção de aplicativo](https://docs.microsoft.com/intune/app-protection-policies).

Requisitos de política de proteção de aplicativo:

- O usuário tem uma licença do Intune ou EMS.
- O usuário pertence a um grupo direcionado pelas políticas de proteção de aplicativos.
- Somente um usuário corporativo está conectado aos aplicativos protegidos em um dispositivo.
- O aplicativo implementou o [SDK do Intune](https://docs.microsoft.com/intune/app-sdk-get-started). Para obter uma lista de aplicativos que oferecem suporte ao SDK, confira [Aplicativos protegidos do Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

As políticas se aplicam depois que um usuário que atende aos requisitos acima se inscreve em um aplicativo habilitado para SDK do Intune. A maneira mais fácil de determinar se uma política é aplicada é exigindo que o usuário defina um PIN na política. 

Para saber mais, confira:

[Perguntas frequentes sobre a solução de problemas do APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Como validar a configuração da política de proteção de aplicativos](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Compreender o tempo de entrega da Política de Proteção de Aplicativos](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Como monitorar políticas de proteção de aplicativos](https://docs.microsoft.com/intune/app-protection-policies-monitor)
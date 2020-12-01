---
title: Erro de licenciamento DLP de ponto de extremidade
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477640"
---
# <a name="endpoint-dlp-licensing-error"></a>Erro de licenciamento DLP de ponto de extremidade

Ao tentar configurar o Endpoint DLP, se você receber o seguinte erro:

`Your organization is missing the licenses required to manage these devices`.

Verifique se você tem uma das seguintes assinaturas ou Complementos:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Conformidade do Microsoft 365 E5
- Conformidade do Microsoft 365 A5
- Governança e Proteção de Informações do Microsoft 365 E5
- Governança e Proteção de Informações do Microsoft 365 A5

> [!NOTE]
> Isso não funcionará para combinações de licença, como: Win E5 + O365 E5 + EMS e5. Você deve ter uma licença simples do M365 E5 para instalar esse recurso.

Para obter mais informações sobre licenciamento do Endpoint DLP, consulte [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)

---
title: Erro de licenciamento de DLP do ponto de extremidade
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
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090115"
---
# <a name="endpoint-dlp-licensing-error"></a>Erro de licenciamento de DLP do ponto de extremidade

Ao tentar configurar a DLP do Ponto de Extremidade, se você receber o seguinte erro:

`Your organization is missing the licenses required to manage these devices`.

Verifique se você tem uma das seguintes assinaturas ou complementos:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Conformidade do Microsoft 365 E5
- Conformidade do Microsoft 365 A5
- Governança e Proteção de Informações do Microsoft 365 E5
- Governança e Proteção de Informações do Microsoft 365 A5

> [!NOTE]
> Isso não funcionará para combinações de licença como: Win E5 + O365 E5 + EMS E5. Você deve ter uma licença M365 E5 pura para configurar esse recurso.

Para obter mais informações de licenciamento de DLP de ponto de extremidade, consulte [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)

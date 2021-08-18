---
title: Enviar notificações personalizadas com o Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086152"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Como enviar notificações personalizadas aos usuários de dispositivos iOS e Android gerenciados

As notificações personalizadas para o Intune são processadas pelo Portal da Empresa aplicativo no dispositivo de um usuário. Em seguida, o aplicativo cria a notificação por push nesse dispositivo.

Veja a seguir os pré-requisitos do dispositivo para dar suporte ao recebimento de notificações personalizadas e para que o aplicativo crie a notificação por push:

- O dispositivo deve ter o aplicativo Portal da Empresa instalado.  

- O dispositivo deve permitir que o Portal da Empresa envie notificações por push. Quando o aplicativo for instalado ou atualizado, ele solicitará que o usuário permita notificações.

- Os dispositivos Android devem ter o Google Play Services instalado.

- O dispositivo deve estar inscrito no Intune.

Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação do recurso](https://docs.microsoft.com/intune/custom-notifications).

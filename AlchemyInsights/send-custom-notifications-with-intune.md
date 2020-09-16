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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720634"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Como enviar notificações personalizadas para os usuários de dispositivos iOS e Android gerenciados

As notificações personalizadas para o Intune são processadas pelo aplicativo do portal da empresa no dispositivo de um usuário. Em seguida, o aplicativo cria a notificação por push nesse dispositivo.

Estes são os pré-requisitos de dispositivo para suportar o recebimento de notificações personalizadas e para o aplicativo criar a notificação por push:

- O dispositivo deve ter o aplicativo portal da empresa instalado.  

- O dispositivo deve permitir que o aplicativo do portal da empresa envie notificações por push. Quando o aplicativo é instalado ou atualizado, ele solicitará que o usuário permita notificações.

- Os dispositivos Android devem ter o Google Play Services instalado.

- O dispositivo deve ser inscrito no Intune.

Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação do recurso](https://docs.microsoft.com/intune/custom-notifications).

---
title: Enviar notificações personalizadas com o Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886845"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Como enviar notificações personalizadas para os usuários de dispositivos iOS e Android gerenciados

As notificações personalizadas para o Intune são processadas pelo aplicativo do portal da empresa no dispositivo de um usuário. Em seguida, o aplicativo cria a notificação por push nesse dispositivo.

Estes são os pré-requisitos de dispositivo para suportar o recebimento de notificações personalizadas e para o aplicativo criar a notificação por push:

- O dispositivo deve ter o aplicativo portal da empresa instalado.  

- O dispositivo deve permitir que o aplicativo do portal da empresa envie notificações por push. Quando o aplicativo é instalado ou atualizado, ele solicitará que o usuário permita notificações.

- Os dispositivos Android devem ter o Google Play Services instalado.

- O dispositivo deve ser inscrito no Intune.

Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação do recurso](https://docs.microsoft.com/intune/custom-notifications).

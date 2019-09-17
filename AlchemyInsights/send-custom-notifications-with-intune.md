---
title: Enviar notificações personalizadas com o Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992301"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Como enviar notificações personalizadas para os usuários de dispositivos iOS e Android gerenciados

As notificações personalizadas para o Intune são processadas pelo aplicativo do portal da empresa no dispositivo de um usuário. Em seguida, o aplicativo cria a notificação por push nesse dispositivo.

Estes são os pré-requisitos de dispositivo para suportar o recebimento de notificações personalizadas e para o aplicativo criar a notificação por push:

- O dispositivo deve ter o aplicativo portal da empresa instalado.  

- O dispositivo deve permitir que o aplicativo do portal da empresa envie notificações por push. Quando o aplicativo é instalado ou atualizado, ele solicitará que o usuário permita notificações.

- Os dispositivos Android devem ter o Google Play Services instalado.

- O dispositivo deve ser inscrito no Intune.

Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação do recurso](https://docs.microsoft.com/intune/custom-notifications).

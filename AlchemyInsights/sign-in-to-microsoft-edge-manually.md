---
title: Entrar no Microsoft Edge manualmente
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599440"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Entrar no Microsoft Edge manualmente

Se um usuário não estiver conectado automaticamente durante uma experiência de primeira execução, o usuário poderá fazer logon manualmente através das configurações do navegador ou do submenu de identidade. Para gerenciar a entrada, use as seguintes políticas:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -para garantir que o usuário sempre tenha um perfil de trabalho no Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -para restringir a entrada a um conjunto de contas confiáveis.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -para desabilitar a entrada ou forçar os usuários a entrar.


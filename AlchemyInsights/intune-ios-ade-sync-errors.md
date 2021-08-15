---
title: Erros de sincronização de registro automático de dispositivo apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013736"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erros de sincronização de registro automático de dispositivo apple

"Detectamos que você tem um ou mais Tokens ADE/DEP que estão em um estado de erro. Até que o estado de erro seja resolvido para cada token afetado, a funcionalidade do ADE não funcionará conforme esperado.".

Esse erro pode se manifesto de várias maneiras, incluindo:

1. Os dispositivos podem não sincronizar entre ABM/ASM e Intune
2. As atribuições de perfil de registro podem estar falhando
3. Os dispositivos podem não concluir o registro do ADE com êxito

Verifique se o erro de sincronização relatado no console do Intune em **Dispositivos > Registrar Dispositivos >** apple registro > tokens de programa de registro .

Uma das causas mais comuns de erro de sincronização é a expiração do token atual. Em muitos casos, a renovação do token afetado resolverá o problema.

Se um ou mais de seus tokens expirar, consulte a documentação a seguir para ajudá-lo a renová-los conforme apropriado:

[Renovar um token de registro de dispositivo automatizado](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Além disso, você pode ver a documentação a seguir para ver possíveis correções de outros erros que causam falhas de sincronização de token:

[ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)

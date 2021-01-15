---
title: Erros de sincronização do Registro Automático de Dispositivo da Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707852"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erros de sincronização do Registro Automático de Dispositivo da Apple

"Detectamos que você tem um ou mais tokens ADE/DEP que estão em um estado de erro. Até que o estado do erro seja resolvido para cada token afetado, a funcionalidade do ADE não funcionará para o mesmo".

Esse erro pode ser manifesto de várias maneiras, incluindo:

1. Os dispositivos podem não ser sincronizados do ABM/ASM para o Intune
2. As atribuições de perfil de registro podem estar falhando
3. Os dispositivos podem não concluir o registro do ADE com êxito

Verifique o erro de sincronização relatado no console do Intune em Dispositivos > Registrar **Dispositivos >** Apple > Tokens de programa de registro da Apple e revise a documentação a seguir para ver qualquer possível correção:

[Erros de sincronização ABM/ASM para tokens de registro automatizado de dispositivos iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)

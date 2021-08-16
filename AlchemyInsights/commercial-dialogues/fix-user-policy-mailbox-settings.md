---
title: Corrigir configurações de política de usuário/caixa de correio
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034706"
---
# <a name="fix-user-policymailbox-settings"></a>Corrigir configurações de política de usuário/caixa de correio

As configurações de lixo eletrônico na caixa de correio afetaram essa mensagem. Para revisar as configurações, faça o seguinte:

1. Iniciar Exchange Shell de Gerenciamento. Para obter mais informações, [consulte Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Execute este comando (usando o endereço de email do usuário):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Verifique se o endereço de email do remetente faz parte **de TrustedSendersAndDomains** ou **BlockedSendersAndDomains**. Se o endereço de email estiver em uma das listas, talvez seja preciso removê-lo. Para saber mais, confira [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).

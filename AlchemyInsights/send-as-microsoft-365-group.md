---
title: Enviar como grupo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086116"
---
# <a name="send-as-microsoft-365-group"></a>Enviar como grupo Microsoft 365

Você pode atribuir permissões de “Enviar como” para permitir que certos usuários enviem mensagens como um grupo Microsoft 365:  

1. Conecte-se ao Exchange Online PowerShell.  

2. Execute o seguinte comando:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Para mais informações, confira [Permitir que os membros enviem email usando “Enviar como” ou “Enviar em nome de um grupo”](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).
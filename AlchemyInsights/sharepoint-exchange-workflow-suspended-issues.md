---
title: Introdução ao SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700695"
---
# <a name="workflows-in-sharepoint"></a>Workflows in SharePoint

Se os fluxos de trabalho do SharePoint não estiverem enviando emails, sua organização pode ter encontrado os limites de remetentes do Exchange Online.

A mensagem de erro "o fluxo de trabalho é suspenso" pode ocorrer se você tiver um dos seguintes itens:

- Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho do SharePoint 2010 ou SharePoint 2013.

- O fluxo de trabalho é configurado para enviar uma mensagem de email personalizada para mais de 200 usuários por vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.

Quando você executa o fluxo de trabalho, a mensagem de email não é enviada e você observa a mensagem de erro, o status interno é definido como suspenso ou não é possível enviar a um destinatário.

Para obter mais informações, consulte o [artigo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)a seguir.


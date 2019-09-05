---
title: Introdução ao SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 4c0220dd2535a1ef41aeef99e2bfc3fe28bac03a
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751660"
---
# <a name="workflows-in-sharepoint"></a>Workflows in SharePoint

Se os fluxos de trabalho do SharePoint não estiverem enviando emails, sua organização pode ter encontrado os limites de remetentes do Exchange Online.

Mensagem de erro "o fluxo de trabalho é suspenso" pode ocorrer se você tiver um dos seguintes itens:

- Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho do SharePoint 2010 ou SharePoint 2013.

- O fluxo de trabalho é configurado para enviar uma mensagem de email personalizada para mais de 200 usuários por vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.

Quando você executa o fluxo de trabalho, a mensagem de email não é enviada e você observa a mensagem de erro, o status interno é definido como suspenso ou não é possível enviar a um destinatário.

Para obter mais informações, consulte o [artigo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)a seguir.


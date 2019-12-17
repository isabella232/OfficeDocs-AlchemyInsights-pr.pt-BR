---
title: Limite de emails diários excedido. O fluxo de trabalho foi suspenso.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053105"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite de emails diários excedido. O fluxo de trabalho foi suspenso.

Esse erro pode ser recebido nos seguintes cenários:

- Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho do SharePoint 2010 ou SharePoint 2013.
- O fluxo de trabalho é configurado para enviar uma mensagem de email personalizada para mais de 200 usuários por vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.
- Quando você executa o fluxo de trabalho, a mensagem de email não é enviada e você observa o seguinte comportamento:
    - Para um fluxo de trabalho usando o tipo de plataforma do SharePoint 2013, navegue até a página **status do fluxo de trabalho** . Na página status do fluxo de trabalho, o **status interno** é definido como **iniciado**e o balão de informações exibe **não é possível enviar a um destinatário**.

Para contornar esse problema, configure seu fluxo de trabalho para enviar mensagens de email sem exceder os [limites de remetentes do Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Por exemplo, use uma pausa no fluxo de trabalho, envie o email para um grupo do Office 365, um grupo de distribuição ou um grupo de segurança habilitado para email ou envie a mensagem para menos de 200 destinatários por vez.


Para obter mais informações, consulte o [artigo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)a seguir.

## <a name="related-topics"></a>Tópicos relacionados
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e fluxo](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
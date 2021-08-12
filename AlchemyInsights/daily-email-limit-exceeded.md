---
title: Limite de email diário excedido. O fluxo de trabalho está suspenso.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914639"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite de email diário excedido. O fluxo de trabalho está suspenso.

Esse erro pode ser recebido nos seguintes cenários:

- Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.
- O fluxo de trabalho é configurado para enviar uma mensagem de email personalizada para mais de 200 usuários por vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.
- Quando você executar o fluxo de trabalho, a mensagem de email não será enviada e você observará o seguinte comportamento:
    - Para um fluxo de trabalho usando o tipo de plataforma SharePoint 2013, navegue até a página **Status do Fluxo de** Trabalho. Na página Status do Fluxo de Trabalho, o **Status Interno** é definido como **Iniciado** e o balão de informações exibe Não é possível enviar para **um destinatário**.

Para resolver esse problema, configure seu fluxo de trabalho para enviar mensagens de email sem exceder os limites Exchange Online [de remetente.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Por exemplo, use uma pausa no fluxo de trabalho, envie o email para um grupo de Microsoft 365, um grupo de distribuição ou um grupo de segurança habilitado para email ou envie a mensagem para menos de 200 destinatários por vez.


Para obter mais informações, consulte o artigo [a seguir](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Tópicos relacionados
- [Criar Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
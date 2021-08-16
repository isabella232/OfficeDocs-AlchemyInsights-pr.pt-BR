---
title: Começar com o SharePoint Online
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
ms.openlocfilehash: a14705003f742641f10c8459b7c7024146e4134a8d5113451e5732cef7326484
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54051402"
---
# <a name="workflows-in-sharepoint"></a>Fluxos de trabalho no SharePoint

Se SharePoint fluxos de trabalho não estão enviando emails, sua organização pode ter encontrado os Exchange Online de remetente.

A mensagem de erro "Fluxo de Trabalho é Suspenso" pode ocorrer se você tiver um dos seguintes itens:

- Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.

- O fluxo de trabalho é configurado para enviar uma mensagem de email personalizada para mais de 200 usuários por vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.

Quando você executar o fluxo de trabalho, a mensagem de email não é enviada e a mensagem de erro, o Status Interno é definido como Suspenso ou Não é possível enviar para um destinatário é exibido.

Para obter mais informações, consulte o seguinte [artigo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).


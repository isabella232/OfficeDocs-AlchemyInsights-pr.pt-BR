---
title: 1048 5.7.750 Serviço indisponível. Cliente impedido de enviar de domínios não-registro
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774239"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 O cliente foi impedido de enviar de um domínio não registrado

O erro ocorre quando um grande volume de mensagens é enviado de domínios que não são provisionados em seu locatário (adicionado como domínios aceitos e validados).

Para evitar esse erro, você pode usar um conector de fluxo de emails baseado em certificado onde o domínio do certificado é um domínio provisionado ou você pode provisionar todos os domínios de envio.

Para saber mais, confira [Corrigir problemas de entrega de email com o código de erro 5.7.700 a 5.7.750 no Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).
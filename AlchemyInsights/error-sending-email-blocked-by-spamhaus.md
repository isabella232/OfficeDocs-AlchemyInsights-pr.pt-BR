---
title: Erro de envio de email bloqueado pelo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783755"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erro ao enviar email: host do cliente bloqueado usando Spamhaus

O endereço IP que enviou a mensagem está em uma lista de bloqueio de Propriedade do [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Os motivos para serem bloqueados pelo Spamhaus incluem contas comprometidas, máquinas comprometidas compartilhando um endereço IP público e políticas de provedor de serviços de Internet. As possíveis correções são:
  
- Para mensagens de entrada bloqueadas nas quais você controla o servidor de email de origem, você precisa determinar a causa e remover o bloco do site do Spamhaus.

- Para mensagens de entrada bloqueadas nas quais o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site do Spamhaus. Se o endereço IP estiver na lista de bloqueio de política (PBL), o proprietário poderá atribuir um endereço IP estático diferente ou remover o endereço do PBL.

- Para mensagens de saída bloqueadas do seu domínio conectado à Microsoft, você poderá receber esse erro se as mensagens forem encaminhadas através de um serviço de terceiros. Você pode usar uma ferramenta de pesquisa WHOIS para localizar o proprietário do endereço IP bloqueado.

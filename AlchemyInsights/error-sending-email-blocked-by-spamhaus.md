---
title: Erro ao enviar email bloqueada pelo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912336"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erro ao enviar email: cliente host bloqueado usando Spamhaus

O endereço IP que enviou a mensagem é em uma lista de bloqueios pertencente a [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Os motivos para que estão sendo bloqueadas pelo Spamhaus incluem contas comprometidas, comprometida máquinas compartilhando um endereço IP público e políticas de provedor de serviços de Internet (ISP). Correções possíveis são:
  
- Bloqueado para mensagens de entrada para o Office 365, onde você pode controlar o servidor de email de origem, você precisará determinar a causa e remover o bloqueio do site Spamhaus.
    
- Bloqueado para mensagens de entrada para o Office 365 onde o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloqueio do site Spamhaus. Se o endereço IP está na lista de bloqueio de política (PBL), o proprietário pode atribuir um endereço IP estático diferente ou remova o endereço do PBL.
    
- Para mensagens de saída bloqueadas do seu domínio do Office 365, você poderá receber esse erro, se as mensagens são roteadas através de um serviço de terceiros 3º. Você pode usar uma ferramenta de pesquisa WHOIS para encontrar o proprietário do endereço IP bloqueado.
    


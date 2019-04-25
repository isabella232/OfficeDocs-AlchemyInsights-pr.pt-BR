---
title: Erro de envio de email bloqueado pelo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402247"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erro ao enviar email: host do cliente bloqueado usando Spamhaus

O endereço IP que enviou a mensagem está em uma lista de bloqueio de Propriedade do [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Os motivos para serem bloqueados pelo Spamhaus incluem contas comprometidas, máquinas comprometidas compartilhando um endereço IP público e políticas de provedor de serviços de Internet. As possíveis correções são:
  
- Para mensagens de entrada bloqueadas para o Office 365, onde você controla o servidor de email de origem, é necessário determinar a causa e remover o bloco do site do Spamhaus.
    
- Para mensagens de entrada bloqueadas para o Office 365, onde o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site do Spamhaus. Se o endereço IP estiver na lista de bloqueio de política (PBL), o proprietário poderá atribuir um endereço IP estático diferente ou remover o endereço do PBL.
    
- Para mensagens de saída bloqueadas do seu domínio do Office 365, você poderá receber esse erro se as mensagens forem encaminhadas através de um serviço de terceiros. Você pode usar uma ferramenta de pesquisa WHOIS para localizar o proprietário do endereço IP bloqueado.
    


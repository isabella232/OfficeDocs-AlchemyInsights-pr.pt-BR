---
title: Não é possível enviar/receber emails do Office 365 devido à desabilitação TLS 1.0 e TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726903"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Não é possível enviar/receber emails do Office 365 devido à desabilitação TLS 1.0 e TLS 1.1

Conforme confirmado pela postagem do centro de mensagens MC229914, a depreciação TLS 1.0 e TLS 1.1 começou a ser imposta para os pontos de extremidade de fluxo de emails do Exchange Online. Em breve, o Office 365 não aceitará mais conexões de email TLS 1.0 e TLS 1.1 de fontes externas. Além disso, o Exchange Online nunca usará o TLS 1.0 ou 1.1 para enviar emails de saída. Se você estiver enfrentando problemas por causa da desabilitação do TLS 1.0 ou 1.1, poderá ter um dos seguintes erros:

- O remetente está recebendo o retorno de NDR - '421 4.4.2 Connection dropped due to SocketError'
- Erro no Visualizador de Filas do servidor local que está enviando emails para o Diretor 365- '421 4.4.2 A conexão caiu devido a SocketError'
- Erro no log de protocolo do conector de [envio](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) no servidor que envia emails para o Office 365- A negociação TLS falhou com o erro SocketError
- Erro no log de protocolo de conector de envio ou recebimento - '451 5.7.3 Deve emitir primeiro um comando STARTTLS'

Se você experimentar qualquer um dos erros acima, verifique se o servidor que está enviando ou recebendo emails tem o TLS 1.2 habilitado verificando as seguintes chaves do Registro-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Se você fizer qualquer alteração nas chaves do Registro acima para habilitar o TLS 1.2, reinicie o servidor para que as alterações entre em vigor. Além disso, certifique-se de ter as atualizações mais recentes do Windows e do Exchange instaladas.

Para mais informações, confira:

- [Exchange Server TLS, parte 1: Preparando-se para o TLS 1.2 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server diretrizes TLS Parte 2: Habilbilando o TLS 1.2 e identificando clientes que não o usam - Comunidade Técnica da Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Noções básicas sobre cenários de email se as versões TLS não puderem ser aceitas com o Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)

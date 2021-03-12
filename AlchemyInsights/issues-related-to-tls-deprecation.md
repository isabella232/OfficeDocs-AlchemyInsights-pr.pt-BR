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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="c48cf-102">Não é possível enviar/receber emails do Office 365 devido à desabilitação TLS 1.0 e TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="c48cf-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="c48cf-103">Conforme confirmado pela postagem do centro de mensagens MC229914, a depreciação TLS 1.0 e TLS 1.1 começou a ser imposta para os pontos de extremidade de fluxo de emails do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c48cf-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="c48cf-104">Em breve, o Office 365 não aceitará mais conexões de email TLS 1.0 e TLS 1.1 de fontes externas.</span><span class="sxs-lookup"><span data-stu-id="c48cf-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="c48cf-105">Além disso, o Exchange Online nunca usará o TLS 1.0 ou 1.1 para enviar emails de saída.</span><span class="sxs-lookup"><span data-stu-id="c48cf-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="c48cf-106">Se você estiver enfrentando problemas por causa da desabilitação do TLS 1.0 ou 1.1, poderá ter um dos seguintes erros:</span><span class="sxs-lookup"><span data-stu-id="c48cf-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="c48cf-107">O remetente está recebendo o retorno de NDR - '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="c48cf-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="c48cf-108">Erro no Visualizador de Filas do servidor local que está enviando emails para o Diretor 365- '421 4.4.2 A conexão caiu devido a SocketError'</span><span class="sxs-lookup"><span data-stu-id="c48cf-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="c48cf-109">Erro no log de protocolo do conector de [envio](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) no servidor que envia emails para o Office 365- A negociação TLS falhou com o erro SocketError</span><span class="sxs-lookup"><span data-stu-id="c48cf-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="c48cf-110">Erro no log de protocolo de conector de envio ou recebimento - '451 5.7.3 Deve emitir primeiro um comando STARTTLS'</span><span class="sxs-lookup"><span data-stu-id="c48cf-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="c48cf-111">Se você experimentar qualquer um dos erros acima, verifique se o servidor que está enviando ou recebendo emails tem o TLS 1.2 habilitado verificando as seguintes chaves do Registro-</span><span class="sxs-lookup"><span data-stu-id="c48cf-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="c48cf-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="c48cf-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="c48cf-113">Se você fizer qualquer alteração nas chaves do Registro acima para habilitar o TLS 1.2, reinicie o servidor para que as alterações entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="c48cf-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="c48cf-114">Além disso, certifique-se de ter as atualizações mais recentes do Windows e do Exchange instaladas.</span><span class="sxs-lookup"><span data-stu-id="c48cf-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="c48cf-115">Para mais informações, confira:</span><span class="sxs-lookup"><span data-stu-id="c48cf-115">For more information, see:</span></span>

- [<span data-ttu-id="c48cf-116">Exchange Server TLS, parte 1: Preparando-se para o TLS 1.2 - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="c48cf-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="c48cf-117">Exchange Server diretrizes TLS Parte 2: Habilbilando o TLS 1.2 e identificando clientes que não o usam - Comunidade Técnica da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c48cf-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="c48cf-118">Noções básicas sobre cenários de email se as versões TLS não puderem ser aceitas com o Exchange Online - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="c48cf-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)

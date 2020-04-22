---
title: Erro de envio de email bloqueado pelo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714246"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="c748b-102">Erro ao enviar email: host do cliente bloqueado usando Spamhaus</span><span class="sxs-lookup"><span data-stu-id="c748b-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="c748b-103">O endereço IP que enviou a mensagem está em uma lista de bloqueio de Propriedade do [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="c748b-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="c748b-104">Os motivos para serem bloqueados pelo Spamhaus incluem contas comprometidas, máquinas comprometidas compartilhando um endereço IP público e políticas de provedor de serviços de Internet.</span><span class="sxs-lookup"><span data-stu-id="c748b-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="c748b-105">As possíveis correções são:</span><span class="sxs-lookup"><span data-stu-id="c748b-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="c748b-106">Para mensagens de entrada bloqueadas nas quais você controla o servidor de email de origem, você precisa determinar a causa e remover o bloco do site do Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="c748b-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="c748b-107">Para mensagens de entrada bloqueadas nas quais o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site do Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="c748b-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="c748b-108">Se o endereço IP estiver na lista de bloqueio de política (PBL), o proprietário poderá atribuir um endereço IP estático diferente ou remover o endereço do PBL.</span><span class="sxs-lookup"><span data-stu-id="c748b-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="c748b-109">Para mensagens de saída bloqueadas do seu domínio conectado à Microsoft, você poderá receber esse erro se as mensagens forem encaminhadas através de um serviço de terceiros.</span><span class="sxs-lookup"><span data-stu-id="c748b-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="c748b-110">Você pode usar uma ferramenta de pesquisa WHOIS para localizar o proprietário do endereço IP bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c748b-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

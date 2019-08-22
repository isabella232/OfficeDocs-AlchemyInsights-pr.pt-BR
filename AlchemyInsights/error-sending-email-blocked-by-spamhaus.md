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
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527120"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f30f1-102">Erro ao enviar email: host do cliente bloqueado usando Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f30f1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f30f1-103">O endereço IP que enviou a mensagem está em uma lista de bloqueio de Propriedade do [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f30f1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f30f1-104">Os motivos para serem bloqueados pelo Spamhaus incluem contas comprometidas, máquinas comprometidas compartilhando um endereço IP público e políticas de provedor de serviços de Internet.</span><span class="sxs-lookup"><span data-stu-id="f30f1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f30f1-105">As possíveis correções são:</span><span class="sxs-lookup"><span data-stu-id="f30f1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f30f1-106">Para mensagens de entrada bloqueadas para o Office 365, onde você controla o servidor de email de origem, é necessário determinar a causa e remover o bloco do site do Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f30f1-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="f30f1-107">Para mensagens de entrada bloqueadas para o Office 365, onde o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site do Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f30f1-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f30f1-108">Se o endereço IP estiver na lista de bloqueio de política (PBL), o proprietário poderá atribuir um endereço IP estático diferente ou remover o endereço do PBL.</span><span class="sxs-lookup"><span data-stu-id="f30f1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="f30f1-109">Para mensagens de saída bloqueadas do seu domínio do Office 365, você poderá receber esse erro se as mensagens forem encaminhadas através de um serviço de terceiros.</span><span class="sxs-lookup"><span data-stu-id="f30f1-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f30f1-110">Você pode usar uma ferramenta de pesquisa WHOIS para localizar o proprietário do endereço IP bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f30f1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

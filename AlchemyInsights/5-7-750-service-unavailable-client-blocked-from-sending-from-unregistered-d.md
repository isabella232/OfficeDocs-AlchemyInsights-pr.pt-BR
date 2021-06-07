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
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="951ff-103">5.7.750 O cliente foi impedido de enviar de um domínio não registrado</span><span class="sxs-lookup"><span data-stu-id="951ff-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="951ff-104">O erro ocorre quando um grande volume de mensagens é enviado de domínios que não são provisionados em seu locatário (adicionado como domínios aceitos e validados).</span><span class="sxs-lookup"><span data-stu-id="951ff-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="951ff-105">Para evitar esse erro, você pode usar um conector de fluxo de emails baseado em certificado onde o domínio do certificado é um domínio provisionado ou você pode provisionar todos os domínios de envio.</span><span class="sxs-lookup"><span data-stu-id="951ff-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="951ff-106">Para saber mais, confira [Corrigir problemas de entrega de email com o código de erro 5.7.700 a 5.7.750 no Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span><span class="sxs-lookup"><span data-stu-id="951ff-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>
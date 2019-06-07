---
title: 1048 o serviço 5.7.750 não está disponível. Cliente impedido de enviar de domínios não registrados
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 9417fef2584e9b81a2ca71cbcc5e23ce093d94e8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751691"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="db49f-103">cliente 5.7.750 impedido de enviar de um domínio não registrado</span><span class="sxs-lookup"><span data-stu-id="db49f-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="db49f-104">O erro ocorre quando um grande volume de mensagens é enviado de domínios que não são provisionados no Office 365 (adicionados como domínios aceitos e validados).</span><span class="sxs-lookup"><span data-stu-id="db49f-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="db49f-105">Para evitar esse erro, você pode usar um conector de fluxo de email baseado em certificado onde o domínio do certificado é um domínio provisionado ou pode provisionar todos os domínios de envio.</span><span class="sxs-lookup"><span data-stu-id="db49f-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

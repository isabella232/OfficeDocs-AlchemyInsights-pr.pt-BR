---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717313"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="7253f-102">Corrigir problemas de entrega de email com o código de erro 5.7.23</span><span class="sxs-lookup"><span data-stu-id="7253f-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="7253f-103">Verifique o registro DNS SPF do seu domínio em um SPF ou verificador de registro DNS disponível publicamente na Web.</span><span class="sxs-lookup"><span data-stu-id="7253f-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="7253f-104">Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do [pool de entrega de alto risco](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="7253f-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="7253f-105">As mensagens no pool de entrega de alto risco não passarão as verificações de SPF e, portanto, não serão aceitas pela organização de email de destino.</span><span class="sxs-lookup"><span data-stu-id="7253f-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="7253f-106">Se o problema persistir, talvez seja necessário entrar em contato com o administrador do host de email para o qual você está tentando enviar emails.</span><span class="sxs-lookup"><span data-stu-id="7253f-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="7253f-107">Anote o erro externo detalhado disponível na mensagem de devolução.</span><span class="sxs-lookup"><span data-stu-id="7253f-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="7253f-108">O suporte da Microsoft pode não conseguir assistência adicional.</span><span class="sxs-lookup"><span data-stu-id="7253f-108">Microsoft support may not be able to assist further.</span></span>

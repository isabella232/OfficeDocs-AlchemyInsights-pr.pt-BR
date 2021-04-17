---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821399"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="cdbcd-102">Corrigir problemas de entrega de email para o código de erro 5.7.23</span><span class="sxs-lookup"><span data-stu-id="cdbcd-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="cdbcd-103">Verifique o registro DNS do SPF para seu domínio em um SPF ou um verificador de registro DNS disponível publicamente na Web.</span><span class="sxs-lookup"><span data-stu-id="cdbcd-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="cdbcd-104">Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e roteada pelo Pool de Entrega de Alto [Risco.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="cdbcd-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="cdbcd-105">As mensagens no Pool de Entrega de Alto Risco não passarão verificações SPF e, portanto, não serão aceitas pela organização de email de destino.</span><span class="sxs-lookup"><span data-stu-id="cdbcd-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="cdbcd-106">Se o problema persistir, talvez seja necessário entrar em contato com o administrador do host de email para o qual você está tentando enviar emails.</span><span class="sxs-lookup"><span data-stu-id="cdbcd-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="cdbcd-107">Anote o erro externo detalhado disponível na mensagem de rejeição.</span><span class="sxs-lookup"><span data-stu-id="cdbcd-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="cdbcd-108">O suporte da Microsoft pode não ser capaz de ajudar ainda mais.</span><span class="sxs-lookup"><span data-stu-id="cdbcd-108">Microsoft support may not be able to assist further.</span></span>

---
title: Solucionar problemas de autenticação SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826403"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="463ec-102">Solucionar problemas de autenticação SMTP</span><span class="sxs-lookup"><span data-stu-id="463ec-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="463ec-103">Se você estiver obtendo erros 5.7.57 ou 5.7.3 ao tentar enviar um e-mail SMTP e autenticar com um cliente ou aplicativo, há algumas coisas que você deve verificar:</span><span class="sxs-lookup"><span data-stu-id="463ec-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="463ec-104">O envio SMTP autenticado pode ser desabilitado no seu locatário ou na caixa de correio que você está tentando usar (verifique as duas configurações).</span><span class="sxs-lookup"><span data-stu-id="463ec-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="463ec-105">Para saber mais, consulte [Habilite ou desabilite o envio SMTP autenticado](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="463ec-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="463ec-106">Verifique se os [Padrões de segurança do Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) estão habilitados para o seu inquérito; se ativado, uma autenticação SMTP usando autenticação básica (também conhecida como herdada; isso usará o nome de usuário e a senha) falhará.</span><span class="sxs-lookup"><span data-stu-id="463ec-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>

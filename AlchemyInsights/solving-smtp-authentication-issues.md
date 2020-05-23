---
title: Solucionar problemas de autenticação SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264309"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="d36c1-102">Solucionar problemas de autenticação SMTP</span><span class="sxs-lookup"><span data-stu-id="d36c1-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="d36c1-103">Se você estiver obtendo erros 5.7.57 ou 5.7.3 ao tentar enviar um e-mail SMTP e autenticar com um cliente ou aplicativo, há algumas coisas que você deve verificar:</span><span class="sxs-lookup"><span data-stu-id="d36c1-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="d36c1-104">O envio SMTP autenticado pode ser desabilitado no seu locatário ou na caixa de correio que você está tentando usar (verifique as duas configurações).</span><span class="sxs-lookup"><span data-stu-id="d36c1-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="d36c1-105">Para saber mais, consulte [Habilite ou desabilite o envio SMTP autenticado](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="d36c1-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="d36c1-106">Verifique se os [Padrões de segurança do Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) estão habilitados para o seu inquérito; se ativado, uma autenticação SMTP usando autenticação básica (também conhecida como herdada; isso usará o nome de usuário e a senha) falhará.</span><span class="sxs-lookup"><span data-stu-id="d36c1-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>

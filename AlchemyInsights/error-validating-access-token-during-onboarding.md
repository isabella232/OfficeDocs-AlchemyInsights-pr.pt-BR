---
title: Ocorreu um erro ao validar o erro de token de acesso durante a integração de análise da área de trabalho
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741112"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="2c368-102">Erro "ocorreu um erro ao validar o token de acesso" durante a integração da análise de desktop</span><span class="sxs-lookup"><span data-stu-id="2c368-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="2c368-103">Esse erro normalmente é observado quando o token de autenticação expira.</span><span class="sxs-lookup"><span data-stu-id="2c368-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="2c368-104">Normalmente, a atualização da página atualiza o token.</span><span class="sxs-lookup"><span data-stu-id="2c368-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="2c368-105">No entanto, esse problema pode persistir se houver políticas de acesso condicional aplicadas à conta que está sendo usada para a análise de desktop integrado.</span><span class="sxs-lookup"><span data-stu-id="2c368-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="2c368-106">Você pode revisar os logs de entrada do Azure AD no portal do Azure para ver se há falhas de logon para a conta que está sendo usada para a integração do desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="2c368-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="2c368-107">Para obter mais informações sobre acesso condicional, visite [Plan Your Conditional Access Deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="2c368-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
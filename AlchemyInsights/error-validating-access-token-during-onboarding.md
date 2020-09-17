---
title: Ocorreu um erro ao validar o erro de token de acesso durante a integração de análise da área de trabalho
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783539"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="c74e1-102">Erro "ocorreu um erro ao validar o token de acesso" durante a integração da análise de desktop</span><span class="sxs-lookup"><span data-stu-id="c74e1-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="c74e1-103">Esse erro normalmente é observado quando o token de autenticação expira.</span><span class="sxs-lookup"><span data-stu-id="c74e1-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="c74e1-104">Normalmente, a atualização da página atualiza o token.</span><span class="sxs-lookup"><span data-stu-id="c74e1-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="c74e1-105">No entanto, esse problema pode persistir se houver políticas de acesso condicional aplicadas à conta que está sendo usada para a análise de desktop integrado.</span><span class="sxs-lookup"><span data-stu-id="c74e1-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="c74e1-106">Você pode revisar os logs de entrada do Azure AD no portal do Azure para ver se há falhas de logon para a conta que está sendo usada para a integração do desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="c74e1-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="c74e1-107">Para obter mais informações sobre acesso condicional, visite [Plan Your Conditional Access Deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="c74e1-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
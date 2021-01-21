---
title: Configurar e estender o tempo de vida do token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911965"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="b294a-102">Configurar e estender o tempo de vida do token</span><span class="sxs-lookup"><span data-stu-id="b294a-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="b294a-103">Você pode especificar o tempo de vida de um acesso, SAML ou token de ID emitido pela plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b294a-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="b294a-104">É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="b294a-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="b294a-105">Para obter mais informações, leia [vida útil configurável do token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="b294a-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="b294a-106">Por exemplo, leia [exemplos de como configurar o tempo de vida dos tokens](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="b294a-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="b294a-107">Para saber como configurar o tempo de vida e a compatibilidade de um token no Azure Active Directory B2C (Azure AD B2C), confira [Configurar tokens no Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="b294a-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="b294a-108">O artigo [Configurar o comportamento da sessão no Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descreve os métodos de SSO (login único) usados no Azure AD B2C e ajuda você a escolher o método SSO mais apropriado ao configurar sua política.</span><span class="sxs-lookup"><span data-stu-id="b294a-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="b294a-109">**Quanto tempo duram os tokens? Por quanto tempo eles são válidos?**</span><span class="sxs-lookup"><span data-stu-id="b294a-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="b294a-110">O tempo de vida dos tokens é de uma hora e a duração da sessão é de 24 horas.</span><span class="sxs-lookup"><span data-stu-id="b294a-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="b294a-111">Isso significa que se nenhuma solicitação tiver sido feita em 24 horas, você precisará fazer logoff novamente antes de solicitar um novo token.</span><span class="sxs-lookup"><span data-stu-id="b294a-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="b294a-112">Após 30 de maio de 2020, nenhum novo locatário será capaz de usar a política Configurble Token Lifetime para configurar a sessão e atualizar tokens.</span><span class="sxs-lookup"><span data-stu-id="b294a-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="b294a-113">A preteração acontecerá dentro de vários meses depois disso, o que significa que deixaremos deeducar a sessão existente e atualizar as opiniões de tokens.</span><span class="sxs-lookup"><span data-stu-id="b294a-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="b294a-114">Você ainda pode configurar o tempo de vida dos tokens de acesso após a preteração.</span><span class="sxs-lookup"><span data-stu-id="b294a-114">You can still configure access token lifetimes after the deprecation.</span></span>







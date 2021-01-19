---
title: Problemas de desconexão
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886767"
---
# <a name="sign-out-issues"></a><span data-ttu-id="3cfdb-102">Problemas de desconexão</span><span class="sxs-lookup"><span data-stu-id="3cfdb-102">Sign-out issues</span></span>

<span data-ttu-id="3cfdb-103">Para resolver problemas relacionados ao logout, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="3cfdb-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="3cfdb-104">Se você ou um usuário estiver sendo logado ou excluído dos aplicativos, siga as orientações dos artigos [Configure o gerenciamento de sessão de autenticação com Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) ou [Duração do token configurável na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="3cfdb-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="3cfdb-105">A maioria dos outros erros ou problemas de desconexão pode ser resolvida com a solução de problemas de integração do Azure Active Directory (Azure AD) com o aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="3cfdb-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="3cfdb-106">Você pode encontrar orientação para uma integração específica acessando esta [coleção de tutoriais para integração de aplicativos com o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), incluindo:</span><span class="sxs-lookup"><span data-stu-id="3cfdb-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="3cfdb-107">Tutoriais de aplicativos SaaS</span><span class="sxs-lookup"><span data-stu-id="3cfdb-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="3cfdb-108">Tutoriais de logon único</span><span class="sxs-lookup"><span data-stu-id="3cfdb-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="3cfdb-109">Tutoriais provisionamento de usuário</span><span class="sxs-lookup"><span data-stu-id="3cfdb-109">User-provisioning tutorials</span></span>
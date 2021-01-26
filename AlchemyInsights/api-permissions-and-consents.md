---
title: Permissões e consentimento da API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951857"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="033e8-102">Permissões e consentimento da API</span><span class="sxs-lookup"><span data-stu-id="033e8-102">API permissions and consent</span></span>

<span data-ttu-id="033e8-103">Os aplicativos que se integram à Plataforma de Identidade da Microsoft seguem um modelo de autorização que oferece aos usuários e administradores controle sobre como os dados podem ser acessados.</span><span class="sxs-lookup"><span data-stu-id="033e8-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="033e8-104">A implementação do modelo de autorização foi atualizada no ponto de extremidade da plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="033e8-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="033e8-105">Ele altera como um aplicativo deve interagir com a Plataforma de Identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="033e8-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="033e8-106">[As permissões e o consentimento no](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ponto de extremidade da Plataforma de Identidade da Microsoft abrangem os conceitos básicos desse modelo de autorização, incluindo escopos, permissões e consentimento.</span><span class="sxs-lookup"><span data-stu-id="033e8-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="033e8-107">A estrutura de consentimento do [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita o desenvolvimento de aplicativos cliente nativos e da Web de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="033e8-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="033e8-108">Esses aplicativos permitem o login por contas de usuário de um locatário do Azure AD diferente do aplicativo em que o aplicativo está registrado.</span><span class="sxs-lookup"><span data-stu-id="033e8-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="033e8-109">Talvez eles também precisem acessar APIs da Web, como a API do Microsoft Graph (para acessar o Azure AD, o Intune e os serviços no Microsoft 365) e outras APIs dos serviços Microsoft, além de suas próprias APIs da Web.</span><span class="sxs-lookup"><span data-stu-id="033e8-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>


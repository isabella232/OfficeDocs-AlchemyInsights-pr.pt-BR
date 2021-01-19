---
title: Problemas de consentimento do administrador
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888284"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="825db-102">Problemas de consentimento do administrador</span><span class="sxs-lookup"><span data-stu-id="825db-102">Admin consent issues</span></span>

1. <span data-ttu-id="825db-103">Habilita o [fluxo de trabalho de consentimento](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) do administrador para permitir que os usuários solicitem aprovação do administrador diretamente da tela de consentimento.</span><span class="sxs-lookup"><span data-stu-id="825db-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="825db-104">Se você ou os usuários do seu aplicativo estão vendo erros inesperados durante o processo de consentimento, consulte este artigo para etapas de solução de problemas: Erro inesperado ao executar o consentimento [para um aplicativo.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="825db-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="825db-105">Saiba mais sobre o consentimento do administrador [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) na plataforma de identidade da [Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)como funciona a solicitação de consentimento e como avaliar uma solicitação de consentimento de administrador para todo [o locatário.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="825db-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="825db-106">Os aplicativos que se integram à Plataforma de Identidade da Microsoft seguem um modelo de autorização que oferece aos usuários e administradores controle sobre como os dados podem ser acessados.</span><span class="sxs-lookup"><span data-stu-id="825db-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="825db-107">A implementação do modelo de autorização foi atualizada no ponto de extremidade da Plataforma de Identidade da Microsoft e altera como um aplicativo deve interagir com a Plataforma de Identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="825db-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="825db-108">Consulte [Permissões e consentimento no](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) ponto de extremidade da Plataforma de Identidade da Microsoft para ter uma visão geral desse modelo de autorização, incluindo escopos, permissões e consentimento.</span><span class="sxs-lookup"><span data-stu-id="825db-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>
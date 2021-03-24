---
title: Segredo do cliente de registro de aplicativo ou problemas de certificado
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123033"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="31a70-102">Segredo do cliente de registro de aplicativo ou problemas de certificado</span><span class="sxs-lookup"><span data-stu-id="31a70-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="31a70-103">O segredo do cliente de aplicativo expirando?</span><span class="sxs-lookup"><span data-stu-id="31a70-103">Application client secret expiring?</span></span>

<span data-ttu-id="31a70-104">Independentemente de como o aplicativo registrado foi criado, seja por meio do processo de registro padrão no portal de Registro de Aplicativos ou se a Entidade de Serviço foi criada em seu locatário usando o consentimento do aplicativo, um novo Segredo do Cliente precisará ser criado antes da expiração do atual e atualizado no código do aplicativo relacionado.</span><span class="sxs-lookup"><span data-stu-id="31a70-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="31a70-105">O período máximo de validade é 2 anos.</span><span class="sxs-lookup"><span data-stu-id="31a70-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="31a70-106">Como lembrete, o valor secreto deve ser gravado, pois ele não ficará mais visível depois de sair da página Registros do aplicativo no portal.</span><span class="sxs-lookup"><span data-stu-id="31a70-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="31a70-107">Para obter mais informações, consulte [Início rápido: Registrar](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) um aplicativo na plataforma de identidade da Microsoft e [práticas recomendadas para a plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="31a70-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="31a70-108">Para saber mais, consulte [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="31a70-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>

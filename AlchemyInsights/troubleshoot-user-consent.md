---
title: Solucionar problemas de consentimento do usuário
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
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007886"
---
# <a name="troubleshoot-user-consent"></a>Solucionar problemas de consentimento do usuário

1. Você pode configurar como os usuários finais consentem com aplicativos por meio do Portal do Azure ou do PowerShell. Confira [Configurações de consentimento do usuário](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para obter mais informações.
1. Um administrador também pode usar a [API do Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para conceder consentimento a permissões delegadas em nome de um único usuário. Para obter mais informações, [consulte Obter acesso em nome de um usuário](https://docs.microsoft.com/graph/auth-v2-user).
1. [Erros de Consentimento do](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)Usuário : este artigo aborda erros que podem ocorrer durante o processo de consentimento para um aplicativo. Se você estiver solucionando problemas de prompts de consentimento inesperados que não contêm mensagens de erro, consulte [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
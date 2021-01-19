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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897684"
---
# <a name="troubleshoot-user-consent"></a>Solucionar problemas de consentimento do usuário

1. Você pode configurar como os usuários finais permitem aplicativos por meio do Portal do Azure ou do PowerShell. Confira [as configurações de consentimento do usuário](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para obter mais informações.
1. Um administrador também pode usar a [API do Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para conceder consentimento para permissões delegadas em nome de um único usuário. Para obter mais informações, [consulte Obter acesso em nome de um usuário.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Erros de consentimento do](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)usuário: este artigo discute erros que podem ocorrer durante o processo de consentimento para um aplicativo. Se você estiver solucionando solicitações de consentimento inesperadas que não contêm mensagens de erro, confira Cenários de [autenticação do Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
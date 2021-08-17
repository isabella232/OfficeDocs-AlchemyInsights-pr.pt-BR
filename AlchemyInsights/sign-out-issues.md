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
ms.openlocfilehash: 938db30acc4a26bd3d0e585090c2f4ba55403b987114ef139fa74d4c2433a219
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050718"
---
# <a name="sign-out-issues"></a>Problemas de desconexão

Para resolver problemas relacionados ao logout, execute as seguintes etapas:

1. Se você ou um usuário estiver sendo logado ou excluído dos aplicativos, siga as orientações dos artigos [Configure o gerenciamento de sessão de autenticação com Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) ou [Duração do token configurável na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. A maioria dos outros erros ou problemas de desconexão pode ser resolvida com a solução de problemas de integração do Azure Active Directory (Azure AD) com o aplicativo específico. Você pode encontrar orientação para uma integração específica acessando esta [coleção de tutoriais para integração de aplicativos com o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), incluindo:
    - Tutoriais de aplicativos SaaS
    - Tutoriais de logon único
    - Tutoriais provisionamento de usuário
---
title: Permissões de API e Processo de Consentimento
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379763"
---
# <a name="api-permissions-and-consent-process"></a>Permissões de API e Processo de Consentimento

Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento. [A referência de permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) lista as permissões associadas a cada conjunto principal de APIs do Microsoft Graph. Ele também fornece orientações sobre como usar as permissões.

**Configurar ou atualizar a entidade de serviço**

- [Criar serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Este artigo mostra como criar um novo objeto servicePrincipal.
- Criar um aplicativo do [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) & entidade de serviço no portal - Este artigo mostra como criar um novo aplicativo e entidade de serviço do Azure Active Directory (Azure AD) que podem ser usados com o controle de acesso baseado em função.
- Aplicativos & entidades de serviço no [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - Este artigo descreve o registro de aplicativos, objetos de aplicativo e entidades de serviço no Azure Active Directory: o que são, como são usados e como estão relacionados uns aos outros.

**Adicionar ou atualizar o registro do aplicativo e fornecer consentimento de administrador**

- [Criar um registro de aplicativo](https://docs.microsoft.com/graph/api/application-post-applications) - Este artigo mostra como criar um novo objeto de aplicativo.
- [Atualizar um registro de aplicativo - permissões de API](https://docs.microsoft.com/graph/api/application-update) - Este artigo mostra como atualizar as propriedades de um objeto de aplicativo.
- [Fornecer consentimento do administrador](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Para consentimento e consentimento do administrador em geral, exigimos que um administrador conceda explicitamente o consentimento.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para provedores de RBAC do Microsoft 365 que suportam várias entidades e vários escopos em uma única atribuição de função. Isso é diferente do *tipo de recurso rbacApplication.* O Microsoft Intune é um exemplo desse provedor RBAC. Uma atribuição de função no Intune pode ter uma matriz de entidades e uma matriz de grupos de escopo. **Isso está em beta, o que significa que ele ainda está em desenvolvimento e não é recomendado para uso na produção.**

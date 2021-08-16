---
title: Problemas com um Recurso ou Entidade de Serviço
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028064"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemas com um Recurso ou Entidade de Serviço

1. Se você estiver apenas começando, os objetos de entidade de serviço e aplicativo no [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) descrevem o registro de aplicativos, objetos de aplicativo e entidades de serviço no Azure Active Directory: o que são, como eles são usados e como estão relacionados uns aos outros. Um cenário de exemplo de vários locatários também é apresentado para ilustrar a relação entre o objeto de aplicativo de um aplicativo e os objetos principais de serviço correspondentes.
2. Você pode saber mais sobre a relação entre aplicativos e entidades de serviço lendo aplicativos e objetos de [entidades de](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)serviço em Azure Active Directory .
3. Como: usar o portal para criar um aplicativo e entidade de serviço do [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) que possam acessar recursos mostra como criar um novo aplicativo do Azure Active Directory (Azure AD) e uma entidade de serviço que pode ser usada com o controle de acesso baseado em função.
4. Com a [API de entidade](https://docs.microsoft.com/graph/api/resources/serviceprincipal)de serviço, você pode gerenciar programaticamente instâncias de aplicativos e controlar o que um aplicativo pode fazer em seu locatário.
5. [Tipo de recurso servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lista todas as propriedades e métodos para o tipo de recurso servicePrincipal.
6. As diferenças de tipo de recurso entre o [Azure AD Graph e](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) o Microsoft Graph realçam as diferenças entre os recursos do Azure AD Graph microsoft Graph. Ele mostra recursos que têm nomes diferentes ou não estão disponíveis; ele também realça os recursos disponíveis na versão beta do Microsoft Graph, mas não na versão v1.0.

**Problemas com usuários convidados**

- Início rápido: adicionar usuários convidados ao seu diretório no portal do [Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) mostra como adicionar um novo usuário convidado ao diretório do Azure AD por meio do portal do Azure, enviar um convite e ver como é o processo de resgate de convite do usuário convidado.
- [Tutorial: Criar fluxos de usuários no Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) mostra como criar alguns fluxos de usuários recomendados usando o portal do Azure. Se você estiver procurando informações sobre como configurar um fluxo de credenciais de senha do proprietário do recurso (ROPC) em seu aplicativo, consulte Configure the resource owner password credentials flow in Azure AD B2C.

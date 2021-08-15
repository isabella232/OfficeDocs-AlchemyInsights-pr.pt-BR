---
title: Problemas de desenvolvimento de aplicativos com APIs
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
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013448"
---
# <a name="issues-developing-applications-with-apis"></a>Problemas de desenvolvimento de aplicativos com APIs

Para começar a usar Azure Active Directory Graph API de Azure Active Directory Graph, consulte o guia de início rápido da API do [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , ou exibir a documentação de referência interativa da API do [Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Fim do suporte para Azure Active Directory Autenticação (ADAL) e API de Graph do Azure AD (AAD Graph)**

A partir de 30 de junho de **2020,** não adicionaremos mais nenhum novo recursos ao ADAL e ao Azure AD Graph. Continuaremos fornecendo suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.

A partir de 30 de junho de **2022**, encerraremos o suporte para o ADAL e o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.

Os aplicativos que usam a ADAL nas versões existentes do sistema operacional continuarão a funcionar após esse período, mas não receberão nenhum suporte técnico ou atualizações de segurança.

Os aplicativos que usam o Azure AD Graph após esse período, podem não receber mais respostas do ponto de extremidade do Azure AD Graph.

**Migração da ADAL**

Recomendamos a atualização para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem os últimos recursos e as atualizações de segurança.

Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está em processo de migração de seus aplicativos para o MSAL até o fim do prazo de suporte, garantindo que eles se beneficiem das melhorias contínuas de segurança e recursos do MSAL.

1. [Leia as perguntas frequentes sobre a ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Saiba mais sobre como migrar aplicativos por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Se você precisar de ajuda para entender qual dos seus aplicativos usa o ADAL, recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.

**Migração do AAD Graph**

Para aplicativos que estão usando o Azure AD Graph, siga nossas diretrizes para migrar o [Azure AD Graph aplicativos](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)para o Microsoft Graph .

1. [Nossa lista de verificação de migração fornece um ponto de partida](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph. Recomendamos que você reveja todos o códigos- fonte de seu aplicativos e, se aplicável, contate os ISVs ou os provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os usos Graph AAD em seu locatário.
1. Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento. A [referência Graph permissões](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) da Microsoft lista as permissões associadas a cada conjunto principal de APIs Graph Microsoft. Ele também fornece orientações sobre como usar as permissões.

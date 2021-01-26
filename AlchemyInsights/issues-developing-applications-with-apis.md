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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951859"
---
# <a name="issues-developing-applications-with-apis"></a>Problemas no desenvolvimento de aplicativos com APIs

Para começar a usar a API do Graph do Azure Active Directory, consulte o guia de início rápido da API do [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ou veja a documentação interativa de referência da API do Graph do [Azure AD.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Fim do suporte para a ADAL (Biblioteca de Autenticação do Azure Active Directory) e a API do Azure AD Graph (AAD Graph)**

**A partir de 30 de junho de 2020,** não adicionaremos mais novos recursos à ADAL e ao Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.

A partir de 30 de junho de **2022,** encerraremos o suporte para a ADAL e o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.

Os aplicativos que usam a ADAL em versões existentes do sistema operacional continuarão a funcionar após esse período, mas não receberão nenhum suporte técnico ou atualizações de segurança.

Os aplicativos que usam o Azure AD Graph após esse período podem não receber mais respostas do ponto de extremidade do Azure AD Graph.

**Migração da ADAL**

Recomendamos atualizar para a Biblioteca de [Autenticação da Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)que tem os recursos e as atualizações de segurança mais recentes.

Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está em processo de migração de seus aplicativos para a MSAL até o prazo final do suporte, garantindo que eles se beneficiem das melhorias contínuas de segurança e recursos da MSAL.

1. [Leia as perguntas frequentes da ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Saiba mais sobre como migrar aplicativos por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Se você precisar de ajuda para entender quais dos seus aplicativos usam a ADAL, recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos que não são da Microsoft ADAL em seu locatário.

**Migração do AAD Graph**

Para aplicativos que estão usando o Azure AD Graph, siga nossas orientações para migrar aplicativos do [Azure AD Graph para o Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. O portal de registro de aplicativo do Azure mostra quais aplicativos estão usando o AAD Graph. Recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todo o uso do AAD Graph em seu locatário.
1. Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento. A [referência de permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lista as permissões associadas a cada conjunto principal de APIs do Microsoft Graph. Ele também fornece orientações sobre como usar as permissões.

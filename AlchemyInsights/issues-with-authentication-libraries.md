---
title: Problemas com bibliotecas de autenticação
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54027992"
---
# <a name="issues-with-authentication-libraries"></a>Problemas com bibliotecas de autenticação

1. [plataforma de identidade da Microsoft de autenticação lista](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) bibliotecas de cliente e middleware compatíveis com a Microsoft.
2. A Biblioteca de Autenticação da Microsoft (MSAL) dá [suporte](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) a vários fluxos de autenticação para uso em diferentes cenários de aplicativos.
3. Para autenticar e adquirir tokens, você inicializa um novo aplicativo cliente público ou confidencial em seu código. Você pode definir várias opções de configuração ao inicializar o aplicativo cliente na Biblioteca de Autenticação da Microsoft (MSAL). Para saber mais, confira [Opções de configuração do aplicativo](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Fim do suporte para Azure Active Directory Autenticação (ADAL) e API de Graph do Azure AD (AAD Graph)**

A partir de 30 de junho de **2020,** não adicionaremos mais nenhum novo recursos ao ADAL e ao Azure AD Graph. Continuaremos fornecendo suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.

A partir de 30 de junho de **2022**, encerraremos o suporte para o ADAL e o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.

Os aplicativos que usam a ADAL nas versões existentes do Sistema Operacional continuarão a funcionar após esse período, mas não *receberão nenhum suporte técnico ou atualizações de segurança*.

Os aplicativos que usam o Azure AD Graph após esse período, podem não receber mais respostas do ponto de extremidade do Azure AD Graph.

**Migração da ADAL**

Recomendamos a atualização para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem os últimos recursos e as atualizações de segurança.

Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está em processo de migração de seus aplicativos para o MSAL até o fim do prazo de suporte, garantindo que eles se beneficiem das melhorias contínuas de segurança e recursos do MSAL.

Para saber mais, confira:

1. [Leia as perguntas frequentes sobre a ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba mais sobre como migrar aplicativos por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se você precisar de ajuda para entender qual dos seus aplicativos usa o ADAL, recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.

**Migração do AAD Graph**

Para aplicativos que estão usando o Azure AD Graph, siga nossas diretrizes para migrar aplicativos do [Azure AD Graph microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph. Recomendamos que você reveja todos o códigos- fonte de seu aplicativos e, se aplicável, contate os ISVs ou os provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os usos Graph AAD em seu locatário.
3. Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento. A [referência Graph permissões](https://docs.microsoft.com/graph/permissions-reference) da Microsoft lista as permissões associadas a cada conjunto principal de APIs Graph Microsoft. Ele também fornece orientações sobre como usar as permissões.

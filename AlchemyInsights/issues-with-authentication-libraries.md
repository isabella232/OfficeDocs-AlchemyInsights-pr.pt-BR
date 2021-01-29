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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037208"
---
# <a name="issues-with-authentication-libraries"></a>Problemas com bibliotecas de autenticação

1. [As bibliotecas de autenticação da plataforma de](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identidade da Microsoft listam bibliotecas de middleware e cliente compatíveis com a Microsoft.
2. A Biblioteca de Autenticação da Microsoft (MSAL) oferece suporte a vários fluxos [de](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) autenticação para uso em diferentes cenários de aplicativos.
3. Para autenticar e adquirir tokens, você inicializa um novo aplicativo cliente público ou confidencial em seu código. Você pode definir várias opções de configuração ao inicializar o aplicativo cliente na Biblioteca de Autenticação da Microsoft (MSAL). Para saber mais, consulte Opções [de configuração do aplicativo.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Fim do suporte para a ADAL (Biblioteca de Autenticação do Azure Active Directory) e a API do Azure AD Graph (AAD Graph)**

**A partir de 30 de junho de 2020,** não adicionaremos mais novos recursos à ADAL e ao Azure AD Graph. Continuaremos dando suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.

A partir de 30 de junho de **2022,** encerraremos o suporte para a ADAL e o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.

Os aplicativos que usam a ADAL em versões *existentes* do sistema operacional continuarão a funcionar após esse período, mas não receberão suporte técnico ou atualizações de segurança.

Os aplicativos que usam o Azure AD Graph após esse período podem não receber mais respostas do ponto de extremidade do Azure AD Graph.

**Migração da ADAL**

Recomendamos a atualização para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem os últimos recursos e as atualizações de segurança.

Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está em processo de migração de seus aplicativos para a MSAL até o prazo final do suporte, garantindo que eles se beneficiarão das melhorias contínuas de segurança e recursos da MSAL.

Para saber mais, confira:

1. [Leia as perguntas frequentes sobre a ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba mais sobre como migrar aplicativos por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se você precisar de ajuda para entender quais dos seus aplicativos usam a ADAL, recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.

**Migração do AAD Graph**

Para aplicativos que estão usando o Azure AD Graph, siga nossas orientações para migrar aplicativos do [Azure AD Graph para o Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph. Recomendamos que você reveja todos o códigos- fonte de seu aplicativos e, se aplicável, contate os ISVs ou os provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todo o uso do AAD Graph em seu locatário.
3. Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento. A [referência de permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) lista as permissões associadas a cada conjunto principal de APIs do Microsoft Graph. Ele também fornece orientações sobre como usar as permissões.

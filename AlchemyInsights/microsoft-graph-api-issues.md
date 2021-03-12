---
title: Problemas de API do Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716191"
---
# <a name="microsoft-graph-api-issues"></a>Problemas de API do Microsoft Graph

Este tópico também pode se aplicar aos desenvolvedores que ainda usam a API do Azure AD Graph. No entanto, é **altamente recomendável** que você use o Microsoft Graph para todos os cenários de gerenciamento de diretório, identidade e acesso.

**Problemas de autenticação ou autorização**

- Se seu aplicativo não conseguir adquirir tokens para chamar o Microsoft Graph, escolha Problema em obter uma categoria de token de acesso **(Autenticação)** do Microsoft Graph para obter ajuda e suporte mais **específicos** neste tópico.
- Se seu aplicativo estiver recebendo erros de autorização **401 ou 403** ao chamar o Microsoft Graph, escolha a categoria Obter um erro de acesso negado **(Autorização)** da API do Microsoft Graph para obter ajuda e suporte mais específicos neste tópico.

**Quero usar o Microsoft Graph, mas não sei por onde começar**

- [Visão geral do Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Visão geral do Gerenciamento de Identidade e Acesso no Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Como começar a criar aplicativos do Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Testar APIs do Microsoft Graph em seu locatário ou um locatário de demonstração

**Quero usar o Microsoft Graph, mas ele dá suporte às APIs de diretório v1.0 de que preciso?**

O Microsoft Graph é a API recomendada para gerenciamento de diretório, identidade e acesso. No entanto, ainda há alguns intervalos entre o que é possível no Azure AD Graph e no Microsoft Graph. Revise os artigos a seguir, que destacam as diferenças mais atualizadas para ajudar na sua escolha:

- [Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferenças de método entre o Azure AD e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**A API que estou chamando não funciona - onde posso fazer mais testes?**

**Microsoft Graph Explorer** - Teste AS APIs do Microsoft Graph em seu locatário ou locatário de demonstração e também confira as consultas de **exemplo** no Microsoft Graph Explorer.

**Meu aplicativo é muito lento e também está sendo acelerada. Que melhorias posso fazer?**

Dependendo do seu cenário, há uma variedade de opções à sua disposição para tornar seu aplicativo mais performante e, em alguns casos, menos propenso a ser acelerada pelo serviço (quando você está fazendo muitas chamadas).

- [Práticas recomendadas do Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitações de lotes](https://docs.microsoft.com/graph/json-batching)
- [Rastrear alterações por meio da consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Obter notificado sobre alterações por meio de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Diretrizes de throttling](https://docs.microsoft.com/graph/throttling)

**Onde posso encontrar mais informações sobre erros e problemas conhecidos?**

- [Informações de resposta de erro do Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemas conhecidos com o Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Onde posso verificar o status de disponibilidade e conectividade do serviço?**

A disponibilidade do serviço e a conectividade dos serviços subjacentes que podem ser acessados por meio do Microsoft Graph podem afetar a disponibilidade geral e o desempenho do Microsoft Graph.

- Para a saúde do serviço do Azure Active Directory, verifique o status dos serviços **de Segurança +** Identidade listados na página de status do [Azure.](https://azure.microsoft.com/status/)
- Para serviços do Office que contribuem com o Microsoft Graph, verifique o status dos serviços listados no Painel de [Saúde do Serviço do Office.](https://portal.office.com/adminportal/home#/servicehealth)

Erros de autorização do Microsoft Graph podem ser resultado de vários problemas diferentes, a maioria deles gera um erro 401 ou 403. Por exemplo, todos os itens a seguir podem levar a erros de autorização:

- [Fluxos de aquisição de token de acesso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) incorretos
- [Escopos de permissão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurados
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Fim do suporte à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph)_* _

_*A partir de 30 de junho de 2020**, não adicionaremos mais novos recursos ao ADAL e ao Azure AD Graph. Continuaremos dando suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.

A partir de 30 de junho de **2022**, encerraremos o suporte para o ADAL e o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.

Os aplicativos que usam o ADAL em versões existentes do sistema operacional continuarão a funcionar após esse tempo, mas não receberão suporte técnico *ou atualizações de segurança.*

Os aplicativos que usam o Azure AD Graph após esse tempo podem não receber mais respostas do ponto de extremidade do Azure AD Graph.

**Migração ADAL**

Recomendamos a atualização para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem os últimos recursos e as atualizações de segurança.

Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está em processo de migração de seus aplicativos para o MSAL até o fim do prazo de suporte, garantindo que eles se beneficiem das melhorias contínuas de segurança e recursos do MSAL.

1. [Leia as perguntas frequentes sobre a ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba mais sobre como migrar aplicativos por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se você precisar de ajuda para entender qual dos seus aplicativos usa o ADAL, recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.

**Migração do AAD Graph**

Para aplicativos que estão usando o Azure AD Graph, siga nossas diretrizes para migrar aplicativos do [Azure AD Graph para o Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nossa lista de verificação de migração fornece um ponto de partida](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph. Recomendamos que você reveja todos o códigos- fonte de seu aplicativos e, se aplicável, contate os ISVs ou os provedores de aplicativos. O suporte da Microsoft também pode fornecer uma lista de todo o uso do AAD Graph em seu locatário.
3. Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento. A [referência de permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) lista as permissões associadas a cada conjunto principal de APIs do Microsoft Graph. Ele também fornece orientações sobre como usar as permissões.

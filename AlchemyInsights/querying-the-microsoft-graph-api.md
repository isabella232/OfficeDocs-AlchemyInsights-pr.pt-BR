---
title: Consultando a API do Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950651"
---
# <a name="querying-the-microsoft-graph-api"></a>Consultando a API do Microsoft Graph

Este tópico também pode se aplicar aos desenvolvedores que ainda usam a API do Azure AD Graph. No entanto, é **altamente recomendável** que você use o Microsoft Graph para todos os cenários de gerenciamento de diretório, identidade e acesso.

**Problemas de autenticação ou autorização**

- Se seu aplicativo não conseguir adquirir tokens para chamar o Microsoft Graph, escolha Problema com a aquisição de uma categoria de token de acesso **(Autenticação)** do Microsoft Graph para obter ajuda e suporte mais **específicos** neste tópico.
- Se seu aplicativo estiver recebendo erros de autorização **401 ou 403** ao chamar o Microsoft Graph, escolha a categoria de API do Microsoft Graph obter um erro de acesso negado **(Autorização)** para obter ajuda e suporte mais específicos neste tópico.

**Quero usar o Microsoft Graph, mas não sei por onde começar**

Para saber mais sobre o Microsoft Graph, confira:

- [Visão geral do Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Visão geral do Gerenciamento de Identidades e Acesso no Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Começar a criar aplicativos do Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Testar as APIs do Microsoft Graph em seu locatário ou em um locatário de demonstração

**Quero usar o Microsoft Graph, mas ele dá suporte às APIs de diretório v1.0 de que preciso?**

O Microsoft Graph é a API recomendada para gerenciamento de diretório, identidade e acesso. No entanto, ainda há algumas lacunas entre o que é possível no Azure AD Graph e no Microsoft Graph. Revise os artigos a seguir, que destacam as diferenças mais atualizadas para ajudar na sua escolha:

- [Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferenças de método entre o Azure AD e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Quando eu consulta o *objeto user,* muitas de suas propriedades estão ausentes**

`GET https://graph.microsoft.com/v1.0/users` retorna apenas 11 propriedades, pois o Microsoft Graph seleciona automaticamente um conjunto padrão de propriedades *do* usuário a ser retornada. Se você precisar de outras *propriedades de* usuário, use $select para escolher as propriedades de que seu aplicativo precisa. Experimente primeiro no **Microsoft Graph Explorer.**

**Alguns valores de propriedade do usuário *são nulos,* embora eu saiba que eles estão definidos**

A explicação mais provável é que o aplicativo tenha sido concedido a *permissão User.ReadBasic.All.* Isso permite que o aplicativo leia um conjunto limitado de propriedades do usuário, retornando todas as outras propriedades como nulas, mesmo que elas tenham sido definidas anteriormente. Tente conceder ao aplicativo *permissão User.Read.All.*

Para saber mais, confira [as permissões de usuário do Microsoft Graph.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Estou tendo problemas para usar parâmetros de consulta OData para filtrar dados em minhas solicitações**

Embora o Microsoft Graph suporte a uma ampla variedade de parâmetros de consulta OData, muitos desses parâmetros não são totalmente suportados por serviços de diretório (recursos que herdam de *directoryObject*) no Microsoft Graph. As mesmas limitações que estavam presentes no Azure AD Graph persistem na maior parte do Microsoft Graph:

1. **Sem suporte:**$count, $search e $filter valores *nulos* ou *não nulos*
2. **Sem suporte:**$filter em determinadas propriedades (consulte tópicos de recursos nos quais as propriedades são filtáveis)
3. **Sem suporte:** paging, filtering e sorting ao mesmo tempo
4. **Sem suporte:** filtrar uma relação. Por exemplo: encontre todos os membros do grupo de engenharia que estão no Reino Unido.
5. **Suporte parcial:**$orderby usuário *(somente* displayName e userPrincipalName) e *grupo*
6. **Suporte parcial**: $filter (dá suporte apenas *a eq* *,* *startswith* ou , e *,* e limitado qualquer *)* suporte, $expand (expandir relações de um único objeto retorna todas as relações, mas expandir uma coleção de relações de objetos é limitado)

Para obter mais informações, [consulte Personalizar respostas com parâmetros de consulta.](https://docs.microsoft.com/graph/query-parameters)

**A API que estou chamando não funciona. Onde posso fazer mais testes?**

**Microsoft Graph Explorer** - Teste as APIs do Microsoft Graph em seu locatário ou em um locatário de demonstração e também confira as consultas de **exemplo** no Microsoft Graph Explorer.

**Quando eu consulta dados, parece que estou com um conjunto de dados incompleto definido**

Se você estiver consultando uma coleção (como *usuários),* o Microsoft Graph usa limites de página do lado do servidor para que os resultados sempre sejam retornados com um tamanho de página padrão. Seu aplicativo deve sempre esperar páginas por meio de coleções retornadas do serviço.

Para saber mais, confira:

- [Práticas recomendadas do Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paginação de dados do Microsoft Graph em seu aplicativo](https://docs.microsoft.com/graph/paging)

**Meu aplicativo está muito lento e também está sendo diminuído. Quais aprimoramentos posso fazer?**

Dependendo do seu cenário, há uma variedade de opções diferentes à sua disposição para tornar seu aplicativo mais bem-desempenho e, em alguns casos, menos propenso a ser throttled pelo serviço (quando você está fazendo muitas chamadas).

Para saber mais, consulte:

- [Práticas recomendadas do Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitações de lote](https://docs.microsoft.com/graph/json-batching)
- [Controlar alterações por meio da consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Ser notificado sobre alterações por meio de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Diretrizes de throttling](https://docs.microsoft.com/graph/throttling)

**Onde posso encontrar mais informações sobre erros e problemas conhecidos?**

- [Informações de resposta a erros do Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemas conhecidos com o Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Onde posso verificar o status de disponibilidade e conectividade do serviço?**

A disponibilidade do serviço e a conectividade dos serviços subjacentes que podem ser acessados por meio do Microsoft Graph podem afetar a disponibilidade e o desempenho gerais do Microsoft Graph.

- Para a saúde do serviço do Azure Active Directory, verifique o status dos serviços de Segurança **+** Identidade listados na página [de status do Azure.](https://azure.microsoft.com/status/)
- Para serviços do Office que contribuem para o Microsoft Graph, verifique o status dos serviços listados no Painel [de Saúde do Serviço do Office.](https://portal.office.com/adminportal/home#/servicehealth)

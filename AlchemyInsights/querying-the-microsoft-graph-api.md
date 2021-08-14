---
title: Consultando a API Graph Microsoft
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923227"
---
# <a name="querying-the-microsoft-graph-api"></a>Consultando a API Graph Microsoft

Este tópico também pode se aplicar aos desenvolvedores que ainda usam a API Graph Azure AD. No entanto, é **altamente recomendável** que você use o Microsoft Graph para todos os cenários de gerenciamento de diretório, identidade e acesso.

**Problemas de autenticação ou autorização**

- Se seu aplicativo não conseguir adquirir **tokens** para chamar o Microsoft Graph, escolha Problema ao obter uma categoria de token de acesso **(autenticação)** do Microsoft Graph para obter ajuda e suporte mais específicos neste tópico.
- Se seu aplicativo estiver recebendo erros de autorização **401 ou 403** ao chamar o Microsoft Graph, escolha a categoria Obter um erro de acesso negado **(Autorização)** da API da Microsoft Graph para obter ajuda e suporte mais específicos neste tópico.

**Quero usar o Microsoft Graph, mas não sei por onde começar**

Para saber mais sobre o Microsoft Graph, consulte:

- [Visão geral do Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Visão geral do Gerenciamento de Identidade e Acesso no Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Como começar a criar aplicativos Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Testar APIs do Microsoft Graph em seu locatário ou um locatário de demonstração

**Quero usar o Microsoft Graph, mas ele dá suporte às APIs de diretório v1.0 de que preciso?**

O Microsoft Graph é a API recomendada para gerenciamento de diretório, identidade e acesso. No entanto, ainda há algumas lacunas entre o que é possível no Azure AD Graph microsoft Graph. Revise os artigos a seguir, que destacam as diferenças mais atualizadas para ajudar na sua escolha:

- [Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferenças de propriedade entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferenças de método entre o Azure AD e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Quando faço uma consulta ao *objeto do usuário,* muitas de suas propriedades estão ausentes**

`GET https://graph.microsoft.com/v1.0/users`retorna apenas 11 propriedades, pois a Microsoft Graph seleciona automaticamente um conjunto padrão de propriedades *do* usuário a ser retornada. Se você precisar de outras *propriedades* de usuário, use $select para escolher as propriedades que seu aplicativo precisa. Experimente primeiro no **Microsoft Graph Explorer.**

**Alguns valores de propriedade do usuário são *nulos,* embora eu saiba que eles estão definidos**

A explicação mais provável é que o aplicativo recebeu a *permissão User.ReadBasic.All.* Isso permite que o aplicativo leia um conjunto limitado de propriedades do usuário, retornando todas as outras propriedades como nulas, mesmo que elas tenham sido definidas anteriormente. Tente conceder ao aplicativo *a permissão User.Read.All.*

Para obter mais informações, consulte [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Estou com problemas ao usar parâmetros de consulta OData para filtrar dados em minhas solicitações**

Embora o Microsoft Graph suporte a uma ampla variedade de parâmetros de consulta OData, muitos desses parâmetros não são totalmente suportados pelos serviços de diretório (recursos que herdam de *directoryObject*) no Microsoft Graph. As mesmas limitações que estavam presentes no Azure AD Graph persistir na maior parte do Microsoft Graph:

1. **Sem suporte**: $count, $search e $filter valores *nulos* ou *não nulos*
2. **Não suportado**: $filter em determinadas propriedades (consulte tópicos de recurso em quais propriedades são filtáveis)
3. **Sem suporte:** paja, filtragem e classificação ao mesmo tempo
4. **Sem suporte:** filtragem em uma relação. Por exemplo: encontre todos os membros do grupo de engenharia que estão no Reino Unido.
5. **Suporte parcial**: $orderby no *usuário* (somente displayName e userPrincipalName) e *grupo*
6. Suporte **parcial**: $filter (suporta apenas *eq* *,* *startswith*, ou *,* e , e , e limitado qualquer *)* suporte, $expand (expandir as relações de um único objeto retorna todas as relações, mas expandir uma coleção de relações de objetos é limitada)

Para obter mais informações, consulte [Personalizar respostas com parâmetros de consulta](https://docs.microsoft.com/graph/query-parameters).

**A API que estou chamando não funciona. Onde posso fazer mais testes?**

**Microsoft Graph Explorer** - Teste as APIs do Microsoft Graph em seu locatário  ou locatário de demonstração e confira também as consultas de exemplo no Microsoft Graph Explorer.

**Quando faço uma consulta para dados, parece que tenho um conjunto de dados incompleto**

Se você estiver consultando uma coleção (como *usuários),* o Microsoft Graph usa limites de página do lado do servidor para que os resultados sempre sejam retornados com um tamanho de página padrão. Seu aplicativo sempre deve esperar página por meio de coleções retornadas do serviço.

Para saber mais, confira:

- [Práticas recomendadas Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Paginação de dados do Microsoft Graph em seu aplicativo](https://docs.microsoft.com/graph/paging)

**Meu aplicativo é muito lento e também está sendo acelerada. Que melhorias posso fazer?**

Dependendo do seu cenário, há uma variedade de opções diferentes à sua disposição para tornar seu aplicativo mais performante e, em alguns casos, menos propenso a ser acelerada pelo serviço (quando você está fazendo muitas chamadas).

Para saber mais, consulte:

- [Práticas recomendadas Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitações de lotes](https://docs.microsoft.com/graph/json-batching)
- [Rastrear alterações por meio da consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Obter notificado sobre alterações por meio de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Diretrizes de throttling](https://docs.microsoft.com/graph/throttling)

**Onde posso encontrar mais informações sobre erros e problemas conhecidos?**

- [Informações Graph de resposta de erro da Microsoft](https://docs.microsoft.com/graph/errors)
- [Problemas conhecidos com o Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Onde posso verificar o status de disponibilidade e conectividade do serviço?**

A disponibilidade do serviço e a conectividade dos serviços subjacentes que podem ser acessados por meio do Microsoft Graph podem afetar a disponibilidade geral e o desempenho do Microsoft Graph.

- Para Azure Active Directory de serviço, verifique o status dos serviços **de Segurança +** Identidade listados na página de status do [Azure.](https://azure.microsoft.com/status/)
- Para Office serviços que contribuem para o Microsoft Graph, verifique o status dos serviços listados no Painel de Office [de Saúde do Serviço.](https://portal.office.com/adminportal/home#/servicehealth)

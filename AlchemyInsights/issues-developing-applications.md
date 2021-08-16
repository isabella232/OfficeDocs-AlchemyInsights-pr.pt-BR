---
title: Problemas no desenvolvimento de aplicativos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013412"
---
# <a name="issues-developing-applications"></a>Problemas no desenvolvimento de aplicativos

Para solucionar os problemas mais comuns ao criar apps do Azure Active Directory (AD), veja os seguintes artigos:

- [Estou tendo problemas para entrar nos aplicativos apenas ao usar o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Não sei como alterar os padrões do tempo de vida do token para o meu aplicativo](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Estou confuso sobre como funciona o consentimento de aplicativo](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Não sei como conceder permissões para o meu aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Não entendo a diferença entre permissões delegadas e de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Fim do suporte à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph)*** _

- A partir de 30 de junho de 2020, não adicionaremos mais nenhum novo recurso à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph). Continuaremos dando suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.

- A partir de 30 de junho de 2022, encerraremos o suporte à ADAL e à AAD Graph, e não forneceremos mais suporte técnico ou atualizações de segurança. Como resultado dessa condição, as implicações são as seguintes:

    - Os aplicativos que usam a ADAL nas versões existentes do sistema operacional continuarão a funcionar após esse período, mas não receberão nenhum suporte técnico ou atualizações de segurança.

    - Os apps que usarem o AAD Graph após esse período, talvez não recebam mais respostas do ponto de extremidade do AAD Graph.

**Migração da ADAL**

Se você estiver usando os apps da Microsoft, recomendamos a atualização para a Biblioteca de Autenticação da Microsoft (MSAL), que tem os últimos recursos e as atualizações de segurança. Essa recomendação se baseia no contexto de início do processo de migração dos apps da Microsoft para a MSAL até o prazo final de suporte. 

A migração dos apps da Microsoft para a MSAL garantirá que os apps se beneficiem das melhorias contínuas nos recursos e na segurança da MSAL.

1. [Leia as perguntas frequentes sobre a ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Saiba mais sobre como migrar aplicativos por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Se precisar de ajuda para entender qual de seus apps usam a ADAL, recomendamos que você reveja todos o códigos-fonte dos apps; se aplicável, procure por provedores independentes de software (ISVs) ou por provedores de app. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.

**Migração do AAD Graph**

Para os aplicativos que usam o AAD Graph, siga nossa orientação para migrar os apps do Azure AD Graph para o Microsoft Graph:

1. [Nossa lista de verificação de migração fornece um ponto de partida](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph. Recomendamos que você reveja todos o códigos-fonte de seus apps e, se aplicável, contate os provedores independentes de software (ISVs) ou os provedores de apps. O suporte da Microsoft também pode fornecer informações sobre o uso do AAD Graph em seu locatário.








---
title: Configurar e estender o tempo de vida do token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: ce100fcc2c62d62477f78e10b3cc9233fc2f5c5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329074"
---
# <a name="configure-and-extend-token-lifetimes"></a>Configurar e estender o tempo de vida do token

Você pode especificar o tempo de vida de um acesso, SAML ou token de ID emitido pela plataforma de identidade da Microsoft. É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização. Para obter mais informações, leia [vida útil configurável do token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Por exemplo, leia [exemplos de como configurar o tempo de vida dos tokens](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Para saber como configurar o tempo de vida e a compatibilidade de um token no Azure Active Directory B2C (Azure AD B2C), confira [Configurar tokens no Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

O artigo [Configurar o comportamento da sessão no Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descreve os métodos de SSO (login único) usados no Azure AD B2C e ajuda você a escolher o método SSO mais apropriado ao configurar sua política.

**Quanto tempo duram os tokens? Por quanto tempo eles são válidos?**

O tempo de vida dos tokens é de uma hora e a duração da sessão é de 24 horas. Isso significa que se nenhuma solicitação tiver sido feita em 24 horas, você precisará fazer logoff novamente antes de solicitar um novo token.

**Observação**: após 30 de maio de 2020, nenhum novo locatário poderá usar a política Configurable Token Lifetime para configurar a sessão e atualizar tokens. A preteração acontecerá dentro de vários meses depois disso, o que significa que deixaremos deeducar a sessão existente e atualizar as opiniões de tokens. Você ainda pode configurar o tempo de vida dos tokens de acesso após a preteração.







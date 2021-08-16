---
title: Problemas com declarações e atributos de token
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012872"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemas com declarações e atributos de token

**Atualizar, configurar ou remover declarações de token**

1. Usando o Azure Active Directory (Azure AD), [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) você pode personalizar o tipo de declaração para a declaração de função no token de resposta que você recebe depois de autorizar um aplicativo.
2. Os desenvolvedores de aplicativos podem usar declarações opcionais em seus aplicativos do Azure AD para especificar quais declarações eles querem em tokens enviados para seu aplicativo. Para obter mais informações, [consulte Fornecer declarações opcionais para seu aplicativo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Configurar declarações de grupo para aplicativos com Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Se estiver usando o Login Único Contínuo em seu aplicativo, consulte personalizar declarações [emitidas no token SAML para aplicativos corporativos.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mapeamento de Atributos de Declarações**

1. Para configurar a política de mapeamento de declarações usando o PowerShell, consulte Personalizar declarações emitidas em tokens para um [aplicativo específico em um locatário (Visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atributos de extensão de esquema de diretório fornecem uma maneira de armazenar dados adicionais em Azure Active Directory em objetos de usuário e outros objetos de diretório, como grupos, detalhes do locatário, entidades de serviço. Somente atributos de extensão em objetos de usuário podem ser usados para emitir declarações para aplicativos. [Usar atributos de extensão de esquema de](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) diretório em declarações descreve como usar atributos de extensão de esquema de diretório para enviar dados do usuário a aplicativos em declarações de token.

Para obter mais informações sobre declarações de token, consulte:

- [Declarações em tokens de acesso](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Declarações em um id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Declarações](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que você pode esperar em tokens de ID e tokens de acesso emitidos pelo Azure AD B2C
- [Referência de declarações de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)

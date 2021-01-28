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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029973"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemas com declarações e atributos de token

**Atualizar, configurar ou remover declarações de token**

1. Usando o Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD), você pode personalizar o tipo de declaração para a declaração de função no token de resposta que você recebe depois de autorizar um aplicativo.
2. Os desenvolvedores de aplicativos podem usar declarações opcionais em seus aplicativos do Azure AD para especificar quais declarações querem em tokens enviados para o aplicativo. Para obter mais informações, [consulte Fornecer declarações opcionais para seu aplicativo.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Configurar declarações de grupo para aplicativos com o Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Se estiver usando o Single Sign-on Contínuo em seu aplicativo, consulte personalizar declarações emitidas no [token SAML para aplicativos empresariais.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mapeamento de atributos de declarações**

1. Para configurar a política de mapeamento de declarações usando o PowerShell, confira Personalizar declarações emitidas em tokens para um [aplicativo específico em um locatário (visualização).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Os atributos de extensão do esquema de diretório fornecem uma maneira de armazenar dados adicionais no Azure Active Directory em objetos de usuário e outros objetos de diretório, como grupos, detalhes do locatário, entidades de serviço. Somente atributos de extensão em objetos de usuário podem ser usados para emitir declarações para aplicativos. [O uso de atributos de extensão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) de esquema de diretório em declarações descreve como usar atributos de extensão de esquema de diretório para enviar dados do usuário a aplicativos em declarações de token.

Para obter mais informações sobre declarações de token, consulte:

- [Declarações em tokens de acesso](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Declarações em um id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Declarações](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que você pode esperar em tokens de ID e tokens de acesso emitidos pelo Azure AD B2C
- [Referência de declarações de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)

---
title: Assassínios SAML (Tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109228"
---
# <a name="saml-assertions-tokens"></a>Assassínios SAML (Tokens)

1. Tokens SAML (Security Assertions Markup Language) são representações XML de declarações. Por padrão, tokens SAML Windows O WCF (Communication Foundation) usa em cenários de segurança federados são emitidos tokens. Para obter mais informações, consulte [SamL Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. A plataforma de identidade da Microsoft emite vários tipos de tokens de segurança no processamento de cada fluxo de autenticação. [A referência de declarações de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descreve o formato, as características de segurança e o conteúdo dos tokens SAML 2.0.
3. Siga as diretrizes em Tempo de Vida útil do token configurável [em](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) plataforma de identidade da Microsoft para entender como configurar o tempo de vida do token.
4. Siga as etapas descritas [neste artigo para](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) entender como configurar a criptografia de token SAML do Azure AD.
5. No Azure AD, você pode configurar opções de assinatura de certificado e o algoritmo de assinatura de certificado. Para obter mais informações, consulte Opções avançadas de assinatura [de certificado no token SAML para aplicativos de galeria em Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

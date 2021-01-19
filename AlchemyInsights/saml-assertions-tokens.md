---
title: Declarações SAML (Tokens)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884552"
---
# <a name="saml-assertions-tokens"></a>Declarações SAML (Tokens)

1. Os tokens SAML (Security Assertions Markup Language) são representações XML de declarações. Por padrão, os tokens SAML que o Windows Communication Foundation (WCF) usa em cenários de segurança federados são tokens emitidos. Para obter mais informações, consulte Tokens e declarações [SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. A plataforma de identidade da Microsoft emite vários tipos de tokens de segurança no processamento de cada fluxo de autenticação. [A referência de declarações de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descreve o formato, as características de segurança e o conteúdo dos tokens SAML 2.0.
3. Siga as orientações em tempo de vida [de token configurável na Plataforma de](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) Identidade da Microsoft para entender como configurar o tempo de vida do token.
4. Siga as etapas descritas [neste artigo para](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) entender como configurar a criptografia de token SAML do Azure AD.
5. No Azure AD, você pode configurar opções de assinatura de certificado e o algoritmo de assinatura de certificado. Para saber mais, confira Opções avançadas de assinatura de certificado no [token SAML para aplicativos de galeria no Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

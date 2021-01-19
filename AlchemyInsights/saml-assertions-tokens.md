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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="b52f4-102">Declarações SAML (Tokens)</span><span class="sxs-lookup"><span data-stu-id="b52f4-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="b52f4-103">Os tokens SAML (Security Assertions Markup Language) são representações XML de declarações.</span><span class="sxs-lookup"><span data-stu-id="b52f4-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="b52f4-104">Por padrão, os tokens SAML que o Windows Communication Foundation (WCF) usa em cenários de segurança federados são tokens emitidos.</span><span class="sxs-lookup"><span data-stu-id="b52f4-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="b52f4-105">Para obter mais informações, consulte Tokens e declarações [SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="b52f4-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="b52f4-106">A plataforma de identidade da Microsoft emite vários tipos de tokens de segurança no processamento de cada fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b52f4-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="b52f4-107">[A referência de declarações de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descreve o formato, as características de segurança e o conteúdo dos tokens SAML 2.0.</span><span class="sxs-lookup"><span data-stu-id="b52f4-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="b52f4-108">Siga as orientações em tempo de vida [de token configurável na Plataforma de](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) Identidade da Microsoft para entender como configurar o tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="b52f4-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="b52f4-109">Siga as etapas descritas [neste artigo para](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) entender como configurar a criptografia de token SAML do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b52f4-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="b52f4-110">No Azure AD, você pode configurar opções de assinatura de certificado e o algoritmo de assinatura de certificado.</span><span class="sxs-lookup"><span data-stu-id="b52f4-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="b52f4-111">Para saber mais, confira Opções avançadas de assinatura de certificado no [token SAML para aplicativos de galeria no Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="b52f4-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

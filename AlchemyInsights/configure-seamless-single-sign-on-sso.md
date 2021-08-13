---
title: Configurar o SSO (Acesso Único Contínuo)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966025"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurar o SSO (Acesso Único Contínuo)

**Configurar aplicativos**

1. Você deve obter os valores do fornecedor de aplicativos. Você pode inserir manualmente os valores ou carregar um arquivo de metadados para extrair o valor dos campos.
2. Muitos aplicativos já foram pré-configurados para funcionar com o Azure AD. Esses aplicativos estão listados na galeria de aplicativos que você pode navegar quando você adiciona um aplicativo ao seu locatário do Azure AD. A [série de início rápido](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) orienta você pelo processo.
3. Para criar um aplicativo que não seja de galeria, você pode clicar em **+ Criar** seu próprio botão Aplicativo e dar um nome ao aplicativo.
    - Por padrão, ele selecionará **Integrar** qualquer outro aplicativo que você não encontrar na galeria, que é a opção correta para aplicativos que não são da galeria.
    - Depois de você **atingir Criar** depois de colocar o nome para o aplicativo, ele criará um novo aplicativo não Enterprise galeria.
    - Em seguida, você pode navegar até Logom Único em **Gerenciar** esse aplicativo e você poderá ver diferentes técnicas para **implementá-lo** em seu ambiente.

**Configurar o SSO contínuo para um aplicativo específico**

Para os aplicativos na galeria, você encontrará instruções detalhadas, passo a passo. Para acessar as etapas, você pode procurar uma lista de todos os tutoriais de configuração do aplicativo em tutoriais de configuração [de aplicativo SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Configurar o SSO baseado em SAML**

1. Início rápido: configurar o logom único baseado em SAML (SSO) para um aplicativo em seu [locatário Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Para saber mais sobre a opção baseada em SAML para um único login, consulte [Understand SAML-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Para saber mais sobre as solicitações e respostas de autenticação SAML 2.0 que o Azure Active Directory (Azure AD) oferece suporte para SSO (single Sign-On), consulte [Protocolo SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)único Sign-On .
4. Para saber como criar e configurar um SSO (SSO) baseado em SAML para seu aplicativo no Azure Active Directory (Azure AD) usando a API do Microsoft Graph, consulte [Configure SAML-based single sign-on for your application using](https://docs.microsoft.com/graph/application-saml-sso-configure-api)the Microsoft Graph API .
5. Para saber como o Azure AD usa o protocolo SAML, consulte Como o plataforma de identidade da Microsoft [usa o protocolo SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Configurar Tokens e Declarações**

1. [Como personalizar declarações emitidas no token SAML para aplicativos corporativos.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Para saber como configurar declarações usando o PowerShell, consulte [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Para saber como configurar declarações opcionais, consulte [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Para saber como usar atributos de extensão de esquema de diretório para enviar dados do usuário a aplicativos em declarações de token, consulte [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Para saber como configurar a vida útil do token, consulte Tempo de vida útil do token configurável no plataforma de identidade da Microsoft [(visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. Configurar políticas de tempo de vida do token [(visualização)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - Neste artigo, passamos por um cenário de política comum que pode ajudá-lo a impor novas regras para o tempo de vida do token. No exemplo, você aprenderá a criar uma política que exija que os usuários se autententem com mais frequência em seu aplicativo Web.

**Solucionar problemas de configuração de SSO**

- Para perguntas frequentes sobre Azure Active Directory um único Sign-On (SSO contínuo), consulte Azure Active Directory Acesso Único [Contínuo: Perguntas frequentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Para solucionar problemas de informações sobre problemas comuns Azure Active Directory (Azure AD) Single Sign-On (SSO contínuo), consulte [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).

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
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402255"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurar o SSO (Acesso Único Contínuo)

**Configurar aplicativos**

1. Você deve obter os valores do fornecedor de aplicativos. Você pode inserir manualmente os valores ou carregar um arquivo de metadados para extrair o valor dos campos.
2. Muitos aplicativos já foram pré-configurados para funcionar com o Azure AD. Esses aplicativos estão listados na galeria de aplicativos que você pode navegar quando você adiciona um aplicativo ao seu locatário do Azure AD. A [série de início rápido](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) orienta você pelo processo.
3. Para criar um aplicativo que não seja de galeria, você pode clicar em **+ Criar** seu próprio botão Aplicativo e dar um nome ao aplicativo.
    - Por padrão, ele selecionará **Integrar** qualquer outro aplicativo que você não encontrar na galeria, que é a opção correta para aplicativos que não são da galeria.
    - Depois de atingir **Criar** depois de colocar o nome para o aplicativo, ele criará um novo Aplicativo Empresarial Não Galeria.
    - Em seguida, você pode navegar até Logom Único em **Gerenciar** esse aplicativo e você poderá ver diferentes técnicas para **implementá-lo** em seu ambiente.

**Configurar o SSO contínuo para um aplicativo específico**

Para os aplicativos na galeria, você encontrará instruções detalhadas, passo a passo. Para acessar as etapas, você pode procurar uma lista de todos os tutoriais de configuração do aplicativo em tutoriais de configuração [de aplicativo SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Configurar o SSO baseado em SAML**

1. Início rápido: configurar o logom único (SSO) baseado em SAML para um aplicativo no locatário do [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Para saber mais sobre a opção baseada em SAML para um único login, consulte [Understand SAML-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Para saber mais sobre as solicitações e respostas de autenticação SAML 2.0 que o Azure Active Directory (Azure AD) oferece suporte para SSO (Single Sign-On), consulte [Protocolo SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)único Sign-On .
4. Para saber como criar e configurar um SSO (SSO) baseado em SAML para seu aplicativo no Azure Active Directory (Azure AD) usando a API do Microsoft Graph, consulte [Configure SAML-based single sign-on for your application using the Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Para saber como o Azure AD usa o protocolo SAML, consulte Como a plataforma de identidade da [Microsoft usa o protocolo SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Configurar Tokens e Declarações**

1. [Como personalizar declarações emitidas no token SAML para aplicativos corporativos.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Para saber como configurar declarações usando o PowerShell, consulte [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Para saber como configurar declarações opcionais, consulte [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Para saber como usar atributos de extensão de esquema de diretório para enviar dados do usuário a aplicativos em declarações de token, consulte [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Para saber como configurar o tempo de vida útil do token, consulte Vida útil de token configurável na plataforma de identidade [da Microsoft (visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. Configurar políticas de tempo de vida do token [(visualização)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - Neste artigo, passamos por um cenário de política comum que pode ajudá-lo a impor novas regras para o tempo de vida do token. No exemplo, você aprenderá a criar uma política que exija que os usuários se autententem com mais frequência em seu aplicativo Web.

**Solucionar problemas de configuração de SSO**

- Para perguntas frequentes sobre o Azure Active Directory Seamless Single Sign-On (SSO contínuo), consulte [Azure Active Directory Seamless Single Sign-On: Perguntas frequentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Para solucionar problemas sobre problemas comuns em relação ao Azure Active Directory (Azure AD) Single Sign-On (SSO contínuo), consulte [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).

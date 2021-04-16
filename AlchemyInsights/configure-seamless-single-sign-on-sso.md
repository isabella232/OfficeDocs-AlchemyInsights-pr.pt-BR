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
# <a name="configure-seamless-single-sign-on-sso"></a><span data-ttu-id="fad8a-102">Configurar o SSO (Acesso Único Contínuo)</span><span class="sxs-lookup"><span data-stu-id="fad8a-102">Configure Seamless Single Sign-on (SSO)</span></span>

<span data-ttu-id="fad8a-103">**Configurar aplicativos**</span><span class="sxs-lookup"><span data-stu-id="fad8a-103">**Configure Applications**</span></span>

1. <span data-ttu-id="fad8a-104">Você deve obter os valores do fornecedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="fad8a-104">You should get the values from the application vendor.</span></span> <span data-ttu-id="fad8a-105">Você pode inserir manualmente os valores ou carregar um arquivo de metadados para extrair o valor dos campos.</span><span class="sxs-lookup"><span data-stu-id="fad8a-105">You can manually enter the values or upload a metadata file to extract the value of the fields.</span></span>
2. <span data-ttu-id="fad8a-106">Muitos aplicativos já foram pré-configurados para funcionar com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fad8a-106">Many apps have already been pre-configured to work with Azure AD.</span></span> <span data-ttu-id="fad8a-107">Esses aplicativos estão listados na galeria de aplicativos que você pode navegar quando você adiciona um aplicativo ao seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fad8a-107">These apps are listed in the gallery of apps that you can browse when you add an app to your Azure AD tenant.</span></span> <span data-ttu-id="fad8a-108">A [série de início rápido](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) orienta você pelo processo.</span><span class="sxs-lookup"><span data-stu-id="fad8a-108">The [quickstart series](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) walks you through the process.</span></span>
3. <span data-ttu-id="fad8a-109">Para criar um aplicativo que não seja de galeria, você pode clicar em **+ Criar** seu próprio botão Aplicativo e dar um nome ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fad8a-109">To create a non-gallery application, you can click on **+ Create your own Application** button and give a name to your Application.</span></span>
    - <span data-ttu-id="fad8a-110">Por padrão, ele selecionará **Integrar** qualquer outro aplicativo que você não encontrar na galeria, que é a opção correta para aplicativos que não são da galeria.</span><span class="sxs-lookup"><span data-stu-id="fad8a-110">By default, it will select **Integrate any other application you don't find in the gallery** which is the correct option for Non-gallery applications.</span></span>
    - <span data-ttu-id="fad8a-111">Depois de atingir **Criar** depois de colocar o nome para o aplicativo, ele criará um novo Aplicativo Empresarial Não Galeria.</span><span class="sxs-lookup"><span data-stu-id="fad8a-111">Once you hit **Create** after putting the name for the application, it will create a new Non-gallery Enterprise Application.</span></span>
    - <span data-ttu-id="fad8a-112">Em seguida, você pode navegar até Logom Único em **Gerenciar** esse aplicativo e você poderá ver diferentes técnicas para **implementá-lo** em seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="fad8a-112">Then, you may navigate to **Single Sign-on** under **Manage** of that application and you will be able to see different techniques for implementing it in your environment.</span></span>

<span data-ttu-id="fad8a-113">**Configurar o SSO contínuo para um aplicativo específico**</span><span class="sxs-lookup"><span data-stu-id="fad8a-113">**Configure Seamless SSO for a specific application**</span></span>

<span data-ttu-id="fad8a-114">Para os aplicativos na galeria, você encontrará instruções detalhadas, passo a passo.</span><span class="sxs-lookup"><span data-stu-id="fad8a-114">For the apps in the gallery you will find detailed, step-by-step, instructions.</span></span> <span data-ttu-id="fad8a-115">Para acessar as etapas, você pode procurar uma lista de todos os tutoriais de configuração do aplicativo em tutoriais de configuração [de aplicativo SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)</span><span class="sxs-lookup"><span data-stu-id="fad8a-115">To access the steps you can browse a list of all app configuration tutorials at [SaaS app configuration tutorials](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).</span></span>

<span data-ttu-id="fad8a-116">**Configurar o SSO baseado em SAML**</span><span class="sxs-lookup"><span data-stu-id="fad8a-116">**Configure SAML-based SSO**</span></span>

1. <span data-ttu-id="fad8a-117">Início rápido: configurar o logom único (SSO) baseado em SAML para um aplicativo no locatário do [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)</span><span class="sxs-lookup"><span data-stu-id="fad8a-117">[Quickstart: Set up SAML-based single sign-on (SSO) for an application in your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).</span></span>
2. <span data-ttu-id="fad8a-118">Para saber mais sobre a opção baseada em SAML para um único login, consulte [Understand SAML-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).</span><span class="sxs-lookup"><span data-stu-id="fad8a-118">To learn more about the SAML-based option for single sign-on, see [Understand SAML-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).</span></span>
3. <span data-ttu-id="fad8a-119">Para saber mais sobre as solicitações e respostas de autenticação SAML 2.0 que o Azure Active Directory (Azure AD) oferece suporte para SSO (Single Sign-On), consulte [Protocolo SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)único Sign-On .</span><span class="sxs-lookup"><span data-stu-id="fad8a-119">To learn about the SAML 2.0 authentication requests and responses that Azure Active Directory (Azure AD) supports for Single Sign-On (SSO), see [Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).</span></span>
4. <span data-ttu-id="fad8a-120">Para saber como criar e configurar um SSO (SSO) baseado em SAML para seu aplicativo no Azure Active Directory (Azure AD) usando a API do Microsoft Graph, consulte [Configure SAML-based single sign-on for your application using the Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).</span><span class="sxs-lookup"><span data-stu-id="fad8a-120">To learn how to create and configure a SAML-based single sign-on (SSO) for your application in Azure Active Directory (Azure AD) using the Microsoft Graph API, see [Configure SAML-based single sign-on for your application using the Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).</span></span>
5. <span data-ttu-id="fad8a-121">Para saber como o Azure AD usa o protocolo SAML, consulte Como a plataforma de identidade da [Microsoft usa o protocolo SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).</span><span class="sxs-lookup"><span data-stu-id="fad8a-121">To learn how Azure AD uses the SAML protocol, see [How the Microsoft identity platform uses the SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).</span></span>

<span data-ttu-id="fad8a-122">**Configurar Tokens e Declarações**</span><span class="sxs-lookup"><span data-stu-id="fad8a-122">**Configure Tokens and Claims**</span></span>

1. <span data-ttu-id="fad8a-123">[Como personalizar declarações emitidas no token SAML para aplicativos corporativos.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="fad8a-123">[How to: customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>
2. <span data-ttu-id="fad8a-124">Para saber como configurar declarações usando o PowerShell, consulte [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="fad8a-124">To learn how to configure claims using PowerShell, see [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
3. <span data-ttu-id="fad8a-125">Para saber como configurar declarações opcionais, consulte [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="fad8a-125">To learn how to configure optional claims, see [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
4. <span data-ttu-id="fad8a-126">Para saber como usar atributos de extensão de esquema de diretório para enviar dados do usuário a aplicativos em declarações de token, consulte [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="fad8a-126">To learn how to use directory schema extension attributes for sending user data to applications in token claims, see [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).</span></span>
5. <span data-ttu-id="fad8a-127">Para saber como configurar o tempo de vida útil do token, consulte Vida útil de token configurável na plataforma de identidade [da Microsoft (visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="fad8a-127">To learn how to configure token lifetimes, see [Configurable token lifetimes in the Microsoft identity platform (preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
6. <span data-ttu-id="fad8a-128">Configurar políticas de tempo de vida do token [(visualização)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - Neste artigo, passamos por um cenário de política comum que pode ajudá-lo a impor novas regras para o tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="fad8a-128">[Configure token lifetime policies (preview)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - In this article, we walk through a common policy scenario that can help you impose new rules for token lifetime.</span></span> <span data-ttu-id="fad8a-129">No exemplo, você aprenderá a criar uma política que exija que os usuários se autententem com mais frequência em seu aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="fad8a-129">In the example, you learn how to create a policy that requires users to authenticate more frequently in your web app.</span></span>

<span data-ttu-id="fad8a-130">**Solucionar problemas de configuração de SSO**</span><span class="sxs-lookup"><span data-stu-id="fad8a-130">**Troubleshoot SSO Configuration**</span></span>

- <span data-ttu-id="fad8a-131">Para perguntas frequentes sobre o Azure Active Directory Seamless Single Sign-On (SSO contínuo), consulte [Azure Active Directory Seamless Single Sign-On: Perguntas frequentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).</span><span class="sxs-lookup"><span data-stu-id="fad8a-131">For frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO), see [Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).</span></span>
- <span data-ttu-id="fad8a-132">Para solucionar problemas sobre problemas comuns em relação ao Azure Active Directory (Azure AD) Single Sign-On (SSO contínuo), consulte [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).</span><span class="sxs-lookup"><span data-stu-id="fad8a-132">For troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), see [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).</span></span>
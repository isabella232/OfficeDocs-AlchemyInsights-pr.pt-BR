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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="75fc2-102">Problemas com declarações e atributos de token</span><span class="sxs-lookup"><span data-stu-id="75fc2-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="75fc2-103">**Atualizar, configurar ou remover declarações de token**</span><span class="sxs-lookup"><span data-stu-id="75fc2-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="75fc2-104">Usando o Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD), você pode personalizar o tipo de declaração para a declaração de função no token de resposta que você recebe depois de autorizar um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75fc2-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="75fc2-105">Os desenvolvedores de aplicativos podem usar declarações opcionais em seus aplicativos do Azure AD para especificar quais declarações querem em tokens enviados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75fc2-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="75fc2-106">Para obter mais informações, [consulte Fornecer declarações opcionais para seu aplicativo.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="75fc2-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="75fc2-107">[Configurar declarações de grupo para aplicativos com o Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="75fc2-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="75fc2-108">Se estiver usando o Single Sign-on Contínuo em seu aplicativo, consulte personalizar declarações emitidas no [token SAML para aplicativos empresariais.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="75fc2-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="75fc2-109">**Mapeamento de atributos de declarações**</span><span class="sxs-lookup"><span data-stu-id="75fc2-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="75fc2-110">Para configurar a política de mapeamento de declarações usando o PowerShell, confira Personalizar declarações emitidas em tokens para um [aplicativo específico em um locatário (visualização).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="75fc2-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="75fc2-111">Os atributos de extensão do esquema de diretório fornecem uma maneira de armazenar dados adicionais no Azure Active Directory em objetos de usuário e outros objetos de diretório, como grupos, detalhes do locatário, entidades de serviço.</span><span class="sxs-lookup"><span data-stu-id="75fc2-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="75fc2-112">Somente atributos de extensão em objetos de usuário podem ser usados para emitir declarações para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="75fc2-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="75fc2-113">[O uso de atributos de extensão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) de esquema de diretório em declarações descreve como usar atributos de extensão de esquema de diretório para enviar dados do usuário a aplicativos em declarações de token.</span><span class="sxs-lookup"><span data-stu-id="75fc2-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="75fc2-114">Para obter mais informações sobre declarações de token, consulte:</span><span class="sxs-lookup"><span data-stu-id="75fc2-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="75fc2-115">Declarações em tokens de acesso</span><span class="sxs-lookup"><span data-stu-id="75fc2-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="75fc2-116">Declarações em um id_token</span><span class="sxs-lookup"><span data-stu-id="75fc2-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="75fc2-117">[Declarações](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que você pode esperar em tokens de ID e tokens de acesso emitidos pelo Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="75fc2-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="75fc2-118">Referência de declarações de token SAML</span><span class="sxs-lookup"><span data-stu-id="75fc2-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)

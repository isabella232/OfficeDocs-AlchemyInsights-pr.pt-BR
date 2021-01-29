---
title: Problemas com bibliotecas de autenticação
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037208"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="97615-102">Problemas com bibliotecas de autenticação</span><span class="sxs-lookup"><span data-stu-id="97615-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="97615-103">[As bibliotecas de autenticação da plataforma de](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identidade da Microsoft listam bibliotecas de middleware e cliente compatíveis com a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="97615-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="97615-104">A Biblioteca de Autenticação da Microsoft (MSAL) oferece suporte a vários fluxos [de](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) autenticação para uso em diferentes cenários de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="97615-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="97615-105">Para autenticar e adquirir tokens, você inicializa um novo aplicativo cliente público ou confidencial em seu código.</span><span class="sxs-lookup"><span data-stu-id="97615-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="97615-106">Você pode definir várias opções de configuração ao inicializar o aplicativo cliente na Biblioteca de Autenticação da Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="97615-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="97615-107">Para saber mais, consulte Opções [de configuração do aplicativo.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="97615-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="97615-108">**Fim do suporte para a ADAL (Biblioteca de Autenticação do Azure Active Directory) e a API do Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="97615-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="97615-109">**A partir de 30 de junho de 2020,** não adicionaremos mais novos recursos à ADAL e ao Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="97615-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="97615-110">Continuaremos dando suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.</span><span class="sxs-lookup"><span data-stu-id="97615-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="97615-111">A partir de 30 de junho de **2022,** encerraremos o suporte para a ADAL e o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="97615-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="97615-112">Os aplicativos que usam a ADAL em versões *existentes* do sistema operacional continuarão a funcionar após esse período, mas não receberão suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="97615-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="97615-113">Os aplicativos que usam o Azure AD Graph após esse período podem não receber mais respostas do ponto de extremidade do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="97615-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="97615-114">**Migração da ADAL**</span><span class="sxs-lookup"><span data-stu-id="97615-114">**ADAL Migration**</span></span>

<span data-ttu-id="97615-115">Recomendamos a atualização para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem os últimos recursos e as atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="97615-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="97615-116">Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está em processo de migração de seus aplicativos para a MSAL até o prazo final do suporte, garantindo que eles se beneficiarão das melhorias contínuas de segurança e recursos da MSAL.</span><span class="sxs-lookup"><span data-stu-id="97615-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="97615-117">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="97615-117">For more information, see:</span></span>

1. [<span data-ttu-id="97615-118">Leia as perguntas frequentes sobre a ADAL</span><span class="sxs-lookup"><span data-stu-id="97615-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="97615-119">Saiba mais sobre como migrar aplicativos por plataforma</span><span class="sxs-lookup"><span data-stu-id="97615-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="97615-120">Se você precisar de ajuda para entender quais dos seus aplicativos usam a ADAL, recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="97615-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="97615-121">O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="97615-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="97615-122">**Migração do AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="97615-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="97615-123">Para aplicativos que estão usando o Azure AD Graph, siga nossas orientações para migrar aplicativos do [Azure AD Graph para o Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="97615-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="97615-124">Nossa lista de verificação de migração fornece um ponto de partida.</span><span class="sxs-lookup"><span data-stu-id="97615-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="97615-125">O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="97615-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="97615-126">Recomendamos que você reveja todos o códigos- fonte de seu aplicativos e, se aplicável, contate os ISVs ou os provedores de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="97615-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="97615-127">O suporte da Microsoft também pode fornecer uma lista de todo o uso do AAD Graph em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="97615-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="97615-128">Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento.</span><span class="sxs-lookup"><span data-stu-id="97615-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="97615-129">A [referência de permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) lista as permissões associadas a cada conjunto principal de APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="97615-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="97615-130">Ele também fornece orientações sobre como usar as permissões.</span><span class="sxs-lookup"><span data-stu-id="97615-130">It also provides guidance about how to use the permissions.</span></span>

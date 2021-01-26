---
title: Problemas de desenvolvimento de aplicativos com APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951859"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="700f5-102">Problemas no desenvolvimento de aplicativos com APIs</span><span class="sxs-lookup"><span data-stu-id="700f5-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="700f5-103">Para começar a usar a API do Graph do Azure Active Directory, consulte o guia de início rápido da API do [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ou veja a documentação interativa de referência da API do Graph do [Azure AD.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="700f5-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="700f5-104">**Fim do suporte para a ADAL (Biblioteca de Autenticação do Azure Active Directory) e a API do Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="700f5-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="700f5-105">**A partir de 30 de junho de 2020,** não adicionaremos mais novos recursos à ADAL e ao Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="700f5-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="700f5-106">Continuaremos a fornecer suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.</span><span class="sxs-lookup"><span data-stu-id="700f5-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="700f5-107">A partir de 30 de junho de **2022,** encerraremos o suporte para a ADAL e o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="700f5-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="700f5-108">Os aplicativos que usam a ADAL em versões existentes do sistema operacional continuarão a funcionar após esse período, mas não receberão nenhum suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="700f5-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="700f5-109">Os aplicativos que usam o Azure AD Graph após esse período podem não receber mais respostas do ponto de extremidade do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="700f5-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="700f5-110">**Migração da ADAL**</span><span class="sxs-lookup"><span data-stu-id="700f5-110">**ADAL Migration**</span></span>

<span data-ttu-id="700f5-111">Recomendamos atualizar para a Biblioteca de [Autenticação da Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)que tem os recursos e as atualizações de segurança mais recentes.</span><span class="sxs-lookup"><span data-stu-id="700f5-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="700f5-112">Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está em processo de migração de seus aplicativos para a MSAL até o prazo final do suporte, garantindo que eles se beneficiem das melhorias contínuas de segurança e recursos da MSAL.</span><span class="sxs-lookup"><span data-stu-id="700f5-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="700f5-113">[Leia as perguntas frequentes da ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="700f5-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="700f5-114">[Saiba mais sobre como migrar aplicativos por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="700f5-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="700f5-115">Se você precisar de ajuda para entender quais dos seus aplicativos usam a ADAL, recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="700f5-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="700f5-116">O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos que não são da Microsoft ADAL em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="700f5-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="700f5-117">**Migração do AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="700f5-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="700f5-118">Para aplicativos que estão usando o Azure AD Graph, siga nossas orientações para migrar aplicativos do [Azure AD Graph para o Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="700f5-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="700f5-119">[Nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="700f5-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="700f5-120">O portal de registro de aplicativo do Azure mostra quais aplicativos estão usando o AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="700f5-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="700f5-121">Recomendamos que você revise todo o código-fonte de seus aplicativos e, se aplicável, entre em contato com quaisquer ISVs ou provedores de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="700f5-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="700f5-122">O suporte da Microsoft também pode fornecer uma lista de todo o uso do AAD Graph em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="700f5-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="700f5-123">Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento.</span><span class="sxs-lookup"><span data-stu-id="700f5-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="700f5-124">A [referência de permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lista as permissões associadas a cada conjunto principal de APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="700f5-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="700f5-125">Ele também fornece orientações sobre como usar as permissões.</span><span class="sxs-lookup"><span data-stu-id="700f5-125">It also provides guidance about how to use the permissions.</span></span>

---
title: Problemas no desenvolvimento de aplicativos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950658"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="245e4-102">Problemas no desenvolvimento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="245e4-102">Issues developing applications</span></span>

<span data-ttu-id="245e4-103">Para solucionar os problemas mais comuns ao criar apps do Azure Active Directory (AD), veja os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="245e4-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="245e4-104">Estou tendo problemas para entrar nos aplicativos apenas ao usar o navegador Chrome</span><span class="sxs-lookup"><span data-stu-id="245e4-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="245e4-105">Não sei como alterar os padrões do tempo de vida do token para o meu aplicativo</span><span class="sxs-lookup"><span data-stu-id="245e4-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="245e4-106">Estou confuso sobre como funciona o consentimento de aplicativo</span><span class="sxs-lookup"><span data-stu-id="245e4-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="245e4-107">Não sei como conceder permissões para o meu aplicativo</span><span class="sxs-lookup"><span data-stu-id="245e4-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="245e4-108">Não entendo a diferença entre permissões delegadas e de aplicativo</span><span class="sxs-lookup"><span data-stu-id="245e4-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="245e4-109">\***Fim do suporte à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="245e4-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="245e4-110">A partir de 30 de junho de 2020, não adicionaremos mais nenhum novo recurso à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="245e4-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="245e4-111">Continuaremos dando suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.</span><span class="sxs-lookup"><span data-stu-id="245e4-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="245e4-112">A partir de 30 de junho de 2022, encerraremos o suporte à ADAL e à AAD Graph, e não forneceremos mais suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="245e4-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="245e4-113">Como resultado dessa condição, as implicações são as seguintes:</span><span class="sxs-lookup"><span data-stu-id="245e4-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="245e4-114">Os aplicativos que usam a ADAL nas versões existentes do sistema operacional continuarão a funcionar após esse período, mas não receberão nenhum suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="245e4-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="245e4-115">Os apps que usarem o AAD Graph após esse período, talvez não recebam mais respostas do ponto de extremidade do AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="245e4-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="245e4-116">_ *Migração da ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="245e4-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="245e4-117">Se você estiver usando os apps da Microsoft, recomendamos a atualização para a Biblioteca de Autenticação da Microsoft (MSAL), que tem os últimos recursos e as atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="245e4-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="245e4-118">Essa recomendação se baseia no contexto de início do processo de migração dos apps da Microsoft para a MSAL até o prazo final de suporte.</span><span class="sxs-lookup"><span data-stu-id="245e4-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="245e4-119">A migração dos apps da Microsoft para a MSAL garantirá que os apps se beneficiem das melhorias contínuas nos recursos e na segurança da MSAL.</span><span class="sxs-lookup"><span data-stu-id="245e4-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="245e4-120">Leia as perguntas frequentes sobre a ADAL</span><span class="sxs-lookup"><span data-stu-id="245e4-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="245e4-121">Saiba mais sobre como migrar aplicativos por plataforma</span><span class="sxs-lookup"><span data-stu-id="245e4-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="245e4-122">Se precisar de ajuda para entender qual de seus apps usam a ADAL, recomendamos que você reveja todos o códigos-fonte dos apps; se aplicável, procure por provedores independentes de software (ISVs) ou por provedores de app.</span><span class="sxs-lookup"><span data-stu-id="245e4-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="245e4-123">O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="245e4-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="245e4-124">**Migração do AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="245e4-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="245e4-125">Para os aplicativos que usam o AAD Graph, siga nossa orientação para migrar os apps do Azure AD Graph para o Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="245e4-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="245e4-126">[Nossa lista de verificação de migração fornece um ponto de partida](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="245e4-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="245e4-127">O portal de registro de aplicativos do Azure mostra quais aplicativos estão usando o AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="245e4-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="245e4-128">Recomendamos que você reveja todos o códigos-fonte de seus apps e, se aplicável, contate os provedores independentes de software (ISVs) ou os provedores de apps.</span><span class="sxs-lookup"><span data-stu-id="245e4-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="245e4-129">O suporte da Microsoft também pode fornecer informações sobre o uso do AAD Graph em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="245e4-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>








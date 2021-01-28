---
title: Problemas de acesso condicional
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013914"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="a933b-102">Problemas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="a933b-102">Conditional access issues</span></span>

<span data-ttu-id="a933b-103">**Resolver problemas com o diagnóstico de entrada**</span><span class="sxs-lookup"><span data-stu-id="a933b-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="a933b-104">Você pode descobrir rapidamente o que aconteceu ou diagnosticar problemas relacionados à login do usuário usando o Diagnóstico [de Logom:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="a933b-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="a933b-105">Inicie o Diagnóstico de entrada.</span><span class="sxs-lookup"><span data-stu-id="a933b-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="a933b-106">Encontre o evento a ser analisado inserindo os detalhes que você tem sobre o usuário, o aplicativo, a hora de entrar, a ID da solicitação ou a ID de correlação.</span><span class="sxs-lookup"><span data-stu-id="a933b-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="a933b-107">Revise os resultados de diagnóstico mostrando os detalhes do que aconteceu e quais ações você pode tomar para fazer alterações (se alguma alteração for necessária).</span><span class="sxs-lookup"><span data-stu-id="a933b-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="a933b-108">**Etapas para solucionar problemas de uma login**</span><span class="sxs-lookup"><span data-stu-id="a933b-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="a933b-109">Navegue até a página de login do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a933b-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="a933b-110">Filtrar entrada por usuário, intervalo de tempo, aplicativo, status, aplicativo cliente e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="a933b-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="a933b-111">Selecione um evento de entrada e veja a guia Acesso Condicional para ver quais políticas foram avaliadas.</span><span class="sxs-lookup"><span data-stu-id="a933b-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="a933b-112">Clique na linha de uma política para exibir os detalhes da política e entender por que ela foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="a933b-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="a933b-113">**Ferramentas para solucionar problemas de uma política de Acesso Condicional**</span><span class="sxs-lookup"><span data-stu-id="a933b-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="a933b-114">O modo somente relatório permite avaliar uma política sem afetar os usuários.</span><span class="sxs-lookup"><span data-stu-id="a933b-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="a933b-115">A ferramenta What-if permite simular eventos de login e ver quais políticas se aplicam.</span><span class="sxs-lookup"><span data-stu-id="a933b-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="a933b-116">O insights e a agenda de relatórios exibem o impacto em tempo real de cada política.</span><span class="sxs-lookup"><span data-stu-id="a933b-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="a933b-117">**Políticas de Proteção de Linha de Base**</span><span class="sxs-lookup"><span data-stu-id="a933b-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="a933b-118">As políticas de Proteção de Linha de Base foram preteridas.</span><span class="sxs-lookup"><span data-stu-id="a933b-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="a933b-119">Eles não estão mais sendo imposto e serão removidos em breve do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a933b-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="a933b-120">Recomendamos a habilitação [de padrões de segurança.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="a933b-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="a933b-121">Para obter mais informações sobre o Acesso Condicional, consulte:</span><span class="sxs-lookup"><span data-stu-id="a933b-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="a933b-122">[Práticas recomendadas para acesso condicional no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condições no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controles no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locais no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="a933b-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>

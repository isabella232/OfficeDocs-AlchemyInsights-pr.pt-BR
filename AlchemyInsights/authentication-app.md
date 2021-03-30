---
title: Aplicativo de autenticação
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403768"
---
# <a name="authentication-app"></a><span data-ttu-id="2057e-102">Aplicativo de autenticação</span><span class="sxs-lookup"><span data-stu-id="2057e-102">Authentication app</span></span>

<span data-ttu-id="2057e-103">Se você for um Administrador Global, poderá descobrir rapidamente o que aconteceu ou diagnosticar problemas relacionados ao login do usuário usando o Diagnóstico de [Entrada.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="2057e-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="2057e-104">Inicie o diagnóstico clicando no botão "[Iniciar Diagnóstico](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)".</span><span class="sxs-lookup"><span data-stu-id="2057e-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="2057e-105">Encontre o evento a ser analisado inserindo os detalhes que você tem sobre o usuário, aplicativo, hora de entrada, ID de solicitação ou ID de correlação.</span><span class="sxs-lookup"><span data-stu-id="2057e-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="2057e-106">Revise os resultados do diagnóstico mostrando os detalhes do que aconteceu e as ações que você pode tomar para fazer alterações, caso sejam necessárias alterações.</span><span class="sxs-lookup"><span data-stu-id="2057e-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="2057e-107">**Verifique o cenário aplicável:**</span><span class="sxs-lookup"><span data-stu-id="2057e-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="2057e-108">Se um usuário não estiver recebendo uma notificação por push no aplicativo Microsoft Authenticator, verifique se eles não são mostrados nos usuários bloqueados do MFA, conforme descrito em Bloquear e [desbloquear usuários](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="2057e-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="2057e-109">Se o usuário não estiver bloqueado para o MFA, mas não receber uma notificação por push, ele poderá abrir o aplicativo Microsoft Authenticator, que puxará as solicitações de aprovação pendentes.</span><span class="sxs-lookup"><span data-stu-id="2057e-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="2057e-110">Como um método alternativo de login, o usuário também pode clicar em Entrar de outra maneira e escolher usar um código de verificação no meu aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2057e-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="2057e-111">O Microsoft Authenticator App é o único método disponível para muitos usuários.</span><span class="sxs-lookup"><span data-stu-id="2057e-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="2057e-112">[Saiba mais sobre os padrões de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), verifique Perguntas frequentes sobre aplicativos [autenticadores](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) para perguntas frequentes e como resolvê-las.</span><span class="sxs-lookup"><span data-stu-id="2057e-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="2057e-113">**Vídeos recomendados**</span><span class="sxs-lookup"><span data-stu-id="2057e-113">**Recommended Videos**</span></span>

<span data-ttu-id="2057e-114">[Como configurar o Aplicativo Autenticador em um novo telefone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="2057e-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>

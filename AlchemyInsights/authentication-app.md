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
# <a name="authentication-app"></a>Aplicativo de autenticação

Se você for um Administrador Global, poderá descobrir rapidamente o que aconteceu ou diagnosticar problemas relacionados ao login do usuário usando o Diagnóstico de [Entrada.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Inicie o diagnóstico clicando no botão "[Iniciar Diagnóstico](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)". 
1. Encontre o evento a ser analisado inserindo os detalhes que você tem sobre o usuário, aplicativo, hora de entrada, ID de solicitação ou ID de correlação.
1. Revise os resultados do diagnóstico mostrando os detalhes do que aconteceu e as ações que você pode tomar para fazer alterações, caso sejam necessárias alterações.

**Verifique o cenário aplicável:**

1. Se um usuário não estiver recebendo uma notificação por push no aplicativo Microsoft Authenticator, verifique se eles não são mostrados nos usuários bloqueados do MFA, conforme descrito em Bloquear e [desbloquear usuários](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Se o usuário não estiver bloqueado para o MFA, mas não receber uma notificação por push, ele poderá abrir o aplicativo Microsoft Authenticator, que puxará as solicitações de aprovação pendentes.
1. Como um método alternativo de login, o usuário também pode clicar em Entrar de outra maneira e escolher usar um código de verificação no meu aplicativo móvel.
1. O Microsoft Authenticator App é o único método disponível para muitos usuários. [Saiba mais sobre os padrões de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), verifique Perguntas frequentes sobre aplicativos [autenticadores](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) para perguntas frequentes e como resolvê-las.
 
**Vídeos recomendados**

[Como configurar o Aplicativo Autenticador em um novo telefone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).

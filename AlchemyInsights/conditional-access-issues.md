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
# <a name="conditional-access-issues"></a>Problemas de acesso condicional

**Resolver problemas com o diagnóstico de entrada**

Você pode descobrir rapidamente o que aconteceu ou diagnosticar problemas relacionados à login do usuário usando o Diagnóstico [de Logom:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Inicie o Diagnóstico de entrada.
1. Encontre o evento a ser analisado inserindo os detalhes que você tem sobre o usuário, o aplicativo, a hora de entrar, a ID da solicitação ou a ID de correlação.
1. Revise os resultados de diagnóstico mostrando os detalhes do que aconteceu e quais ações você pode tomar para fazer alterações (se alguma alteração for necessária).

**Etapas para solucionar problemas de uma login** 

1. Navegue até a página de login do Azure AD.
1. Filtrar entrada por usuário, intervalo de tempo, aplicativo, status, aplicativo cliente e assim por diante.
1. Selecione um evento de entrada e veja a guia Acesso Condicional para ver quais políticas foram avaliadas.
1. Clique na linha de uma política para exibir os detalhes da política e entender por que ela foi aplicada.

**Ferramentas para solucionar problemas de uma política de Acesso Condicional**

- O modo somente relatório permite avaliar uma política sem afetar os usuários.
- A ferramenta What-if permite simular eventos de login e ver quais políticas se aplicam.
- O insights e a agenda de relatórios exibem o impacto em tempo real de cada política.

**Políticas de Proteção de Linha de Base**

As políticas de Proteção de Linha de Base foram preteridas. Eles não estão mais sendo imposto e serão removidos em breve do portal do Azure. Recomendamos a habilitação [de padrões de segurança.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Para obter mais informações sobre o Acesso Condicional, consulte:

[Práticas recomendadas para acesso condicional no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condições no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controles no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locais no Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)

---
title: Problemas para entrar nos aplicativos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886769"
---
# <a name="issues-signing-in-to-applications"></a>Problemas para entrar nos aplicativos

Para detectar a causa ou diagnosticar problemas relacionados à login do usuário, execute as seguintes etapas:

1. Inicie o [Diagnóstico de entrada](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Encontre o evento para analisar inserindo os detalhes que você tem sobre o usuário, o aplicativo, a hora de entrar, a ID de solicitação ou a ID de correlação.
3. Revise os resultados do diagnóstico mostrando os detalhes do que aconteceu e as ações que você pode tomar para fazer alterações, caso sejam necessárias alterações.

Veja a seguir alguns problemas comuns que você pode ter ao entrar nos aplicativos:

1. Você ou o usuário **concluiu uma inscrição do Azure AD, mas está vendo um aviso inesperado** – Consulte os artigos [Solicitação de consentimento inesperada ao entrar em um aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) e [Erro inesperado ao executar o consentimento para um aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Você ou um usuário **entrou diretamente em um aplicativo, mas não consegue entrar nele a partir de um deeplink no portal personalizado ou no painel de acesso**: Consulte [Solucionar problemas de entrada em um aplicativo pelo Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Você ou um usuário **concluiu uma inscrição no Azure AD, mas o aplicativo exibe uma mensagem de erro e não permite que o usuário termine o fluxo de login**: O problema é que o aplicativo não aceitou a resposta emitida pelo Azure AD. Siga [estas etapas](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) para solução de problemas.
4. Você ou um usuário **não consegue entrar em um aplicativo que não seja de galeria configurado para o acesso único de senha**: Siga as orientações [estas etapas](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) para solucionar problemas.
5. Você ou um usuário **não consegue entrar em um aplicativo da Galeria Azure AD configurado para o acesso único de senha**: Siga [estas etapas](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) para solucionar problemas.
6. Você ou um usuário **não consegue entrar em um aplicativo da Microsoft**: Siga [estas etapas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) para solucionar problemas.
7. Você ou um usuário **não consegue entrar em um aplicativo que não seja de galeria configurado para o acesso único de senha**: Siga [estas etapas](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) para solucionar problemas.
8. Você ou um usuário **não consegue entrar em um aplicativo da Galeria Azure AD configurado para o acesso único federado**: Siga [estas etapas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) para solucionar problemas.
9. Você ou um usuário **não consegue entrar em um aplicativo personalizado**: Siga [estas etapas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) para solucionar problemas.
10. Você ou um usuário **não consegue entrar em um aplicativo local usando o proxy do aplicativo Azure AD**: Siga [estas etapas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) para solucionar problemas.

